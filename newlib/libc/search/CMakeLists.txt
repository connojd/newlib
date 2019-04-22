#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/bsd_qsort_r.c
    ${CMAKE_CURRENT_LIST_DIR}/bsearch.c
    ${CMAKE_CURRENT_LIST_DIR}/extern.h
    ${CMAKE_CURRENT_LIST_DIR}/hash_bigkey.c
    ${CMAKE_CURRENT_LIST_DIR}/hash_buf.c
    ${CMAKE_CURRENT_LIST_DIR}/hash.c
    ${CMAKE_CURRENT_LIST_DIR}/hash_func.c
    ${CMAKE_CURRENT_LIST_DIR}/hash.h
    ${CMAKE_CURRENT_LIST_DIR}/db_local.h
    ${CMAKE_CURRENT_LIST_DIR}/hash_log2.c
    ${CMAKE_CURRENT_LIST_DIR}/hash_page.c
    ${CMAKE_CURRENT_LIST_DIR}/hcreate.c
    ${CMAKE_CURRENT_LIST_DIR}/hcreate_r.c
    ${CMAKE_CURRENT_LIST_DIR}/page.h
    ${CMAKE_CURRENT_LIST_DIR}/qsort.c
    ${CMAKE_CURRENT_LIST_DIR}/qsort_r.c
    ${CMAKE_CURRENT_LIST_DIR}/tdelete.c
    ${CMAKE_CURRENT_LIST_DIR}/tdestroy.c
    ${CMAKE_CURRENT_LIST_DIR}/tfind.c
    ${CMAKE_CURRENT_LIST_DIR}/tsearch.c
    ${CMAKE_CURRENT_LIST_DIR}/twalk.c
)
