#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/asiprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/asniprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/asnprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/asprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/clearerr.c
    ${CMAKE_CURRENT_LIST_DIR}/clearerr_u.c
    ${CMAKE_CURRENT_LIST_DIR}/diprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/dprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/fcloseall.c
    ${CMAKE_CURRENT_LIST_DIR}/fclose.c
    ${CMAKE_CURRENT_LIST_DIR}/fdopen.c
    ${CMAKE_CURRENT_LIST_DIR}/feof.c
    ${CMAKE_CURRENT_LIST_DIR}/feof_u.c
    ${CMAKE_CURRENT_LIST_DIR}/ferror.c
    ${CMAKE_CURRENT_LIST_DIR}/ferror_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fflush.c
    ${CMAKE_CURRENT_LIST_DIR}/fflush_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fgetc.c
    ${CMAKE_CURRENT_LIST_DIR}/fgetc_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fgetpos.c
    ${CMAKE_CURRENT_LIST_DIR}/fgets.c
    ${CMAKE_CURRENT_LIST_DIR}/fgets_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fgetwc.c
    ${CMAKE_CURRENT_LIST_DIR}/fgetwc_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fgetws.c
    ${CMAKE_CURRENT_LIST_DIR}/fgetws_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fileno.c
    ${CMAKE_CURRENT_LIST_DIR}/fileno_u.c
    ${CMAKE_CURRENT_LIST_DIR}/findfp.c
    ${CMAKE_CURRENT_LIST_DIR}/fiprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/fiscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/flags.c
    ${CMAKE_CURRENT_LIST_DIR}/floatio.h
    ${CMAKE_CURRENT_LIST_DIR}/fmemopen.c
    ${CMAKE_CURRENT_LIST_DIR}/fopen.c
    ${CMAKE_CURRENT_LIST_DIR}/fopencookie.c
    ${CMAKE_CURRENT_LIST_DIR}/fprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/fpurge.c
    ${CMAKE_CURRENT_LIST_DIR}/fputc.c
    ${CMAKE_CURRENT_LIST_DIR}/fputc_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fputs.c
    ${CMAKE_CURRENT_LIST_DIR}/fputs_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fputwc.c
    ${CMAKE_CURRENT_LIST_DIR}/fputwc_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fputws.c
    ${CMAKE_CURRENT_LIST_DIR}/fputws_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fread.c
    ${CMAKE_CURRENT_LIST_DIR}/fread_u.c
    ${CMAKE_CURRENT_LIST_DIR}/freopen.c
    ${CMAKE_CURRENT_LIST_DIR}/fscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/fseek.c
    ${CMAKE_CURRENT_LIST_DIR}/fseeko.c
    ${CMAKE_CURRENT_LIST_DIR}/fsetlocking.c
    ${CMAKE_CURRENT_LIST_DIR}/fsetpos.c
    ${CMAKE_CURRENT_LIST_DIR}/ftell.c
    ${CMAKE_CURRENT_LIST_DIR}/ftello.c
    ${CMAKE_CURRENT_LIST_DIR}/funopen.c
    ${CMAKE_CURRENT_LIST_DIR}/fvwrite.c
    ${CMAKE_CURRENT_LIST_DIR}/fvwrite.h
    ${CMAKE_CURRENT_LIST_DIR}/fwalk.c
    ${CMAKE_CURRENT_LIST_DIR}/fwide.c
    ${CMAKE_CURRENT_LIST_DIR}/fwprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/fwrite.c
    ${CMAKE_CURRENT_LIST_DIR}/fwrite_u.c
    ${CMAKE_CURRENT_LIST_DIR}/fwscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/getc.c
    ${CMAKE_CURRENT_LIST_DIR}/getchar.c
    ${CMAKE_CURRENT_LIST_DIR}/getchar_u.c
    ${CMAKE_CURRENT_LIST_DIR}/getc_u.c
    ${CMAKE_CURRENT_LIST_DIR}/getdelim.c
    ${CMAKE_CURRENT_LIST_DIR}/getline.c
    ${CMAKE_CURRENT_LIST_DIR}/gets.c
    ${CMAKE_CURRENT_LIST_DIR}/getw.c
    ${CMAKE_CURRENT_LIST_DIR}/getwc.c
    ${CMAKE_CURRENT_LIST_DIR}/getwchar.c
    ${CMAKE_CURRENT_LIST_DIR}/getwchar_u.c
    ${CMAKE_CURRENT_LIST_DIR}/getwc_u.c
    ${CMAKE_CURRENT_LIST_DIR}/iprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/iscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/local.h
    ${CMAKE_CURRENT_LIST_DIR}/makebuf.c
    ${CMAKE_CURRENT_LIST_DIR}/mktemp.c
    ${CMAKE_CURRENT_LIST_DIR}/open_memstream.c
    ${CMAKE_CURRENT_LIST_DIR}/perror.c
    ${CMAKE_CURRENT_LIST_DIR}/printf.c
    ${CMAKE_CURRENT_LIST_DIR}/putc.c
    ${CMAKE_CURRENT_LIST_DIR}/putchar.c
    ${CMAKE_CURRENT_LIST_DIR}/putchar_u.c
    ${CMAKE_CURRENT_LIST_DIR}/putc_u.c
    ${CMAKE_CURRENT_LIST_DIR}/puts.c
    ${CMAKE_CURRENT_LIST_DIR}/putw.c
    ${CMAKE_CURRENT_LIST_DIR}/putwc.c
    ${CMAKE_CURRENT_LIST_DIR}/putwchar.c
    ${CMAKE_CURRENT_LIST_DIR}/putwchar_u.c
    ${CMAKE_CURRENT_LIST_DIR}/putwc_u.c
    ${CMAKE_CURRENT_LIST_DIR}/refill.c
    ${CMAKE_CURRENT_LIST_DIR}/remove.c
    ${CMAKE_CURRENT_LIST_DIR}/rename.c
    ${CMAKE_CURRENT_LIST_DIR}/rewind.c
    ${CMAKE_CURRENT_LIST_DIR}/rget.c
    ${CMAKE_CURRENT_LIST_DIR}/scanf.c
    ${CMAKE_CURRENT_LIST_DIR}/sccl.c
    ${CMAKE_CURRENT_LIST_DIR}/setbuf.c
    ${CMAKE_CURRENT_LIST_DIR}/setbuffer.c
    ${CMAKE_CURRENT_LIST_DIR}/setlinebuf.c
    ${CMAKE_CURRENT_LIST_DIR}/setvbuf.c
    ${CMAKE_CURRENT_LIST_DIR}/siprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/siscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/sniprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/snprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/sprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/sscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/stdio.c
    ${CMAKE_CURRENT_LIST_DIR}/stdio_ext.c
    ${CMAKE_CURRENT_LIST_DIR}/swprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/swscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/tmpfile.c
    ${CMAKE_CURRENT_LIST_DIR}/tmpnam.c
    ${CMAKE_CURRENT_LIST_DIR}/ungetc.c
    ${CMAKE_CURRENT_LIST_DIR}/ungetwc.c
    ${CMAKE_CURRENT_LIST_DIR}/vasiprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vasniprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vasnprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vasprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vdiprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vdprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vfieeefp.h
    ${CMAKE_CURRENT_LIST_DIR}/viprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/viscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/vprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/vsiprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vsiscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/vsniprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vsnprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vsprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vsscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/vswprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vswscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/vwprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/vwscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/wbuf.c
    ${CMAKE_CURRENT_LIST_DIR}/wprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/wscanf.c
    ${CMAKE_CURRENT_LIST_DIR}/wsetup.c
)

add_library(io INTERFACE)
target_compile_features(io INTERFACE c_std_11)
target_compile_definitions(io INTERFACE MALLOC_PROVIDED _COMPILING_NEWLIB)
target_compile_definitions(io INTERFACE __NO_SYSCALLS__ MISSING_SYSCALL_NAMES)
target_include_directories(io SYSTEM INTERFACE
    $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/../include>
    $<INSTALL_INTERFACE:include>
)

macro(add_io_lib NAME SRC)
    add_library(${NAME} OBJECT)
    target_sources(${NAME} PRIVATE ${CMAKE_CURRENT_LIST_DIR}/${SRC}.c)
    target_link_libraries(${NAME} PRIVATE io)
    target_link_libraries(c PRIVATE ${NAME})
endmacro(add_io_lib)

# printf
#
add_io_lib(vfprintf vfprintf)
add_io_lib(vfiprintf vfprintf)
add_io_lib(svfprintf vfprintf)
add_io_lib(svfiprintf vfprintf)

target_compile_definitions(vfiprintf PRIVATE INTEGER_ONLY)
target_compile_definitions(svfprintf PRIVATE STRING_ONLY)
target_compile_definitions(svfiprintf PRIVATE INTEGER_ONLY STRING_ONLY)

# wprintf
#
add_io_lib(vfwprintf vfwprintf)
add_io_lib(vfiwprintf vfwprintf)
add_io_lib(svfwprintf vfwprintf)
add_io_lib(svfiwprintf vfwprintf)

target_compile_definitions(vfiwprintf PRIVATE INTEGER_ONLY)
target_compile_definitions(svfwprintf PRIVATE STRING_ONLY)
target_compile_definitions(svfiwprintf PRIVATE INTEGER_ONLY STRING_ONLY)

# scanf
#
add_io_lib(vfscanf vfscanf)
add_io_lib(vfiscanf vfscanf)
add_io_lib(svfscanf vfscanf)
add_io_lib(svfiscanf vfscanf)

target_compile_definitions(vfiscanf PRIVATE INTEGER_ONLY)
target_compile_definitions(svfscanf PRIVATE STRING_ONLY)
target_compile_definitions(svfiscanf PRIVATE INTEGER_ONLY STRING_ONLY)

# wscanf
#
add_io_lib(vfwscanf vfwscanf)
add_io_lib(vfiwscanf vfwscanf)
add_io_lib(svfwscanf vfwscanf)
add_io_lib(svfiwscanf vfwscanf)

target_compile_definitions(vfiwscanf PRIVATE INTEGER_ONLY)
target_compile_definitions(svfwscanf PRIVATE STRING_ONLY)
target_compile_definitions(svfiwscanf PRIVATE INTEGER_ONLY STRING_ONLY)
