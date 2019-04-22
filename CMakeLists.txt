#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

cmake_minimum_required(VERSION 3.13)
project(newlib VERSION 3.0.0)

enable_language(ASM)
set(BUILD_SHARED_LIBS OFF)

# Bareflank-specific defines. These are referenced by the configure_file
# commands below, so they have to be set before those commands.

set(_MB_LEN_MAX 1)
set(_ICONV_ENABLED 1)
set(HAVE_INITFINI_ARRAY 1)
set(_ATEXIT_DYNAMIC_ALLOC 1)
set(_HAVE_LONG_DOUBLE 1)
set(_FVWRITE_IN_STREAMIO 1)
set(_FSEEK_OPTIMIZATION 1)
set(_WIDE_ORIENT 1)
set(_UNBUF_STREAM_OPT 1)

set(SRC ${CMAKE_CURRENT_LIST_DIR})
set(TARG_INC ${PROJECT_BINARY_DIR}/targ-include)

execute_process(COMMAND ${CMAKE_COMMAND} -E make_directory ${TARG_INC}/sys)
execute_process(COMMAND ${CMAKE_COMMAND} -E make_directory ${TARG_INC}/bits)
execute_process(COMMAND ${CMAKE_COMMAND} -E make_directory ${TARG_INC}/machine)

configure_file(
    ${SRC}/cmake/_newlib_version.h.in
    ${SRC}/newlib/libc/include/_newlib_version.h
)

configure_file(
    ${SRC}/cmake/newlib.h.in
    ${SRC}/newlib/libc/include/newlib.h
)

add_subdirectory(newlib/libc)
add_subdirectory(newlib/libm)
