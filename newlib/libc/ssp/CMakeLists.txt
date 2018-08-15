add_library(ssp STATIC "")

target_include_directories(ssp
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)

target_sources(ssp
    PRIVATE
        chk_fail.c
        gets_chk.c
        memcpy_chk.c
        memmove_chk.c
        mempcpy_chk.c
        memset_chk.c
        snprintf_chk.c
        sprintf_chk.c
        stack_protector.c
        stpcpy_chk.c
        stpncpy_chk.c
        strcat_chk.c
        strcpy_chk.c
        strncat_chk.c
        strncpy_chk.c
        vsnprintf_chk.c
        vsprintf_chk.c
)
