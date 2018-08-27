# Copyright (C) 2018 Connor Davis
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

add_library(m STATIC "")
set_target_properties(m PROPERTIES LINKER_LANGUAGE C)

target_compile_features(m
    PRIVATE
        c_std_11
)

target_include_directories(m
    PUBLIC
        $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/../libc/include>
        $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/common>
        $<INSTALL_INTERFACE:include>
)

target_compile_options(m
    PRIVATE
        -msse
        -msse2
        -msse3
        -mno-red-zone
        -mstackrealign
        -fpic
        -fstack-protector-strong
        -U__STRICT_ANSI__
)

target_compile_definitions(m
    PRIVATE
        MALLOC_PROVIDED
        _COMPILING_NEWLIB
    PUBLIC
        CLOCK_MONOTONIC
        _HAVE_LONG_DOUBLE
        _LDBL_EQ_DBL
        _POSIX_TIMERS
        _POSIX_THREADS
        _POSIX_PRIORITY_SCHEDULING
        _UNIX98_THREAD_MUTEX_ATTRIBUTES
        __SINGLE_THREAD__
        __ELF__
        __USER_LABEL_PREFIX__=
)

add_subdirectory(common)
add_subdirectory(complex)
add_subdirectory(machine/i386)
add_subdirectory(math)

#
# Add m target to newlib export set
#
install(
    TARGETS m
    EXPORT newlib::lib
    ARCHIVE DESTINATION lib
    INCLUDES DESTINATION include
)

install(
    DIRECTORY ${CMAKE_CURRENT_LIST_DIR}/../libc/include/
    DESTINATION include
)

# TODO make sure sources aren't installed. Install .h files in src dirs as necessary (fdlibm)
