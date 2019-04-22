#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/memcpy.S
    ${CMAKE_CURRENT_LIST_DIR}/memset.S
    ${CMAKE_CURRENT_LIST_DIR}/setjmp.S
    ${CMAKE_CURRENT_LIST_DIR}/x86_64mach.h
)
