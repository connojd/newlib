# Copyright (C) 2018 Connor Davis
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

add_library(c STATIC "")
set_target_properties(c PROPERTIES LINKER_LANGUAGE C)

target_compile_features(c
    PRIVATE
        c_std_11
)

target_include_directories(c
    PUBLIC
        $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/include>
        $<INSTALL_INTERFACE:include>
)

target_compile_options(c
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

target_compile_definitions(c
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

add_subdirectory(argz)
add_subdirectory(ctype)
add_subdirectory(errno)
add_subdirectory(locale)
add_subdirectory(machine/x86_64)
add_subdirectory(misc)
add_subdirectory(search)
add_subdirectory(signal)
add_subdirectory(ssp)
add_subdirectory(string)
add_subdirectory(time)
add_subdirectory(stdio)
add_subdirectory(stdlib)

#
# Add c target to newlib export set
#
install(
    TARGETS c
    EXPORT newlib::lib
    ARCHIVE DESTINATION lib
    INCLUDES DESTINATION include
)

install(
    DIRECTORY ${CMAKE_CURRENT_LIST_DIR}/include/
    DESTINATION include
)
