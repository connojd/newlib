enable_language(ASM)
add_library(machine STATIC "")

target_sources(machine
    PRIVATE
        x86_64/memcpy.S
        x86_64/memset.S
        x86_64/setjmp.S
        x86_64/x86_64mach.h
)

set_target_properties(machine PROPERTIES LINKER_LANGUAGE C)
