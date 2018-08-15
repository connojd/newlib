add_library(locale STATIC "")

target_include_directories(locale
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)

target_sources(locale
    PRIVATE
        duplocale.c
        freelocale.c
        lctype.c
        lmessages.c
        lmonetary.c
        lnumeric.c
        locale.c
        localeconv.c
        newlocale.c
        nl_langinfo.c
        setlocale.h
        timelocal.c
        uselocale.c
)
