#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/__dprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/ffs.c
    ${CMAKE_CURRENT_LIST_DIR}/fini.c
    ${CMAKE_CURRENT_LIST_DIR}/init.c
    ${CMAKE_CURRENT_LIST_DIR}/lock.c
    ${CMAKE_CURRENT_LIST_DIR}/unctrl.c
)
