add_library(argz STATIC "")

target_include_directories(argz
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)

target_sources(argz
    PRIVATE
        argz_add.c
        argz_add_sep.c
        argz_append.c
        argz_count.c
        argz_create.c
        argz_create_sep.c
        argz_delete.c
        argz_extract.c
        argz_insert.c
        argz_next.c
        argz_replace.c
        argz_stringify.c
        buf_findstr.c
        buf_findstr.h
        dummy.c
        envz_add.c
        envz_entry.c
        envz_get.c
        envz_merge.c
        envz_remove.c
        envz_strip.c
)
