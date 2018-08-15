
add_library(search STATIC "")

target_include_directories(search
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)

target_sources(search
    PRIVATE
        bsd_qsort_r.c
        bsearch.c
        extern.h
        hash_bigkey.c
        hash_buf.c
        hash.c
        hash_func.c
        hash.h
        db_local.h
        hash_log2.c
        hash_page.c
        hcreate.c
        hcreate_r.c
        page.h
        qsort.c
        qsort_r.c
        tdelete.c
        tdestroy.c
        tfind.c
        tsearch.c
        twalk.c
)
