add_library(time STATIC "")

target_include_directories(time
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)

target_sources(time
    PRIVATE
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
        tzcalc_limits.c
        tzlock.c
        tzset.c
        tzset_r.c
        tzvars.c
        wcsftime.c
)
