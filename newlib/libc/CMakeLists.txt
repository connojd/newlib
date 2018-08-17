# Copyright (C) 2018 by Connor Davis
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

enable_language(ASM)
add_library(c STATIC "")
set_target_properties(c PROPERTIES LINKER_LANGUAGE C)

target_compile_features(c
    PRIVATE
        c_std_11
)

target_include_directories(c
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
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
add_subdirectory(machine)
add_subdirectory(misc)
add_subdirectory(search)
add_subdirectory(signal)
add_subdirectory(ssp)
add_subdirectory(string)
add_subdirectory(time)
add_subdirectory(stdio)
add_subdirectory(stdlib)

#
# unused
#

# iconv
# stdio64
# posix
# sys
# reent
# syscalls
# unix
# xdr
