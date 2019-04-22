#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(m PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/f_atan2f.S
    ${CMAKE_CURRENT_LIST_DIR}/f_atan2.S
    ${CMAKE_CURRENT_LIST_DIR}/f_exp.c
    ${CMAKE_CURRENT_LIST_DIR}/f_expf.c
    ${CMAKE_CURRENT_LIST_DIR}/f_frexpf.S
    ${CMAKE_CURRENT_LIST_DIR}/f_frexp.S
    ${CMAKE_CURRENT_LIST_DIR}/f_ldexpf.S
    ${CMAKE_CURRENT_LIST_DIR}/f_ldexp.S
    ${CMAKE_CURRENT_LIST_DIR}/f_llrint.c
    ${CMAKE_CURRENT_LIST_DIR}/f_llrintf.c
    ${CMAKE_CURRENT_LIST_DIR}/f_log10f.S
    ${CMAKE_CURRENT_LIST_DIR}/f_log10.S
    ${CMAKE_CURRENT_LIST_DIR}/f_logf.S
    ${CMAKE_CURRENT_LIST_DIR}/f_log.S
    ${CMAKE_CURRENT_LIST_DIR}/f_lrint.c
    ${CMAKE_CURRENT_LIST_DIR}/f_lrintf.c
    ${CMAKE_CURRENT_LIST_DIR}/f_math.h
    ${CMAKE_CURRENT_LIST_DIR}/f_pow.c
    ${CMAKE_CURRENT_LIST_DIR}/f_powf.c
    ${CMAKE_CURRENT_LIST_DIR}/f_rint.c
    ${CMAKE_CURRENT_LIST_DIR}/f_rintf.c
    ${CMAKE_CURRENT_LIST_DIR}/f_tanf.S
    ${CMAKE_CURRENT_LIST_DIR}/f_tan.S
    ${CMAKE_CURRENT_LIST_DIR}/i386mach.h
)
