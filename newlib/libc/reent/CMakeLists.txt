add_library(reent STATIC "")

target_include_directories(reent
    PUBLIC
        $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/newlib/libc/include>
        $<INSTALL_INTERFACE:include>
)

target_sources(reent
    PRIVATE
        closer.c
        execr.c
        fcntlr.c
        fstat64r.c
        fstatr.c
        getreent.c
        gettimeofdayr.c
        impure.c
        isattyr.c
        linkr.c
        lseek64r.c
        lseekr.c
        mkdirr.c
        open64r.c
        openr.c
        readr.c
        reent.c
        renamer.c
        sbrkr.c
        signalr.c
        signgam.c
        stat64r.c
        statr.c
        timesr.c
        unlinkr.c
        writer.c
)
