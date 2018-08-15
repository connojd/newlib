add_library(misc STATIC "")

target_include_directories(misc
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)

target_sources(misc
    PRIVATE
        __dprintf.c
        ffs.c
        fini.c
        init.c
        lock.c
        unctrl.c
)
