#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/argz_add.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_add_sep.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_append.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_count.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_create.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_create_sep.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_delete.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_extract.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_insert.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_next.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_replace.c
    ${CMAKE_CURRENT_LIST_DIR}/argz_stringify.c
    ${CMAKE_CURRENT_LIST_DIR}/buf_findstr.c
    ${CMAKE_CURRENT_LIST_DIR}/buf_findstr.h
    ${CMAKE_CURRENT_LIST_DIR}/dummy.c
    ${CMAKE_CURRENT_LIST_DIR}/envz_add.c
    ${CMAKE_CURRENT_LIST_DIR}/envz_entry.c
    ${CMAKE_CURRENT_LIST_DIR}/envz_get.c
    ${CMAKE_CURRENT_LIST_DIR}/envz_merge.c
    ${CMAKE_CURRENT_LIST_DIR}/envz_remove.c
    ${CMAKE_CURRENT_LIST_DIR}/envz_strip.c
)
