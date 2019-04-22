#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

target_sources(c PRIVATE
    asctime.c
    asctime_r.c
    clock.c
    ctime.c
    ctime_r.c
    difftime.c
    gettzinfo.c
    gmtime.c
    gmtime_r.c
    lcltime.c
    lcltime_r.c
    local.h
    mktime.c
    month_lengths.c
    strftime.c
    strptime.c
    time.c
    time.tex
    tzcalc_limits.c
    tzlock.c
    tzset.c
    tzset_r.c
    tzvars.c
    wcsftime.c
)
