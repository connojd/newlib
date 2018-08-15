add_library(errno STATIC errno.c)

target_include_directories(errno
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)
