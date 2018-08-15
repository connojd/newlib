add_library(signal STATIC "")

target_include_directories(signal
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)

target_sources(signal
    PRIVATE
        psignal.c
        raise.c
        signal.c
)
