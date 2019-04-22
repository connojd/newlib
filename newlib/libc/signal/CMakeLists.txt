#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/psignal.c
    ${CMAKE_CURRENT_LIST_DIR}/raise.c
    ${CMAKE_CURRENT_LIST_DIR}/signal.c
)
