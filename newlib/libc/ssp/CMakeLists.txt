#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/chk_fail.c
    ${CMAKE_CURRENT_LIST_DIR}/gets_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/memcpy_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/memmove_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/mempcpy_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/memset_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/snprintf_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/sprintf_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/stack_protector.c
    ${CMAKE_CURRENT_LIST_DIR}/stpcpy_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/stpncpy_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/strcat_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/strcpy_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/strncat_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/strncpy_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/vsnprintf_chk.c
    ${CMAKE_CURRENT_LIST_DIR}/vsprintf_chk.c
)
