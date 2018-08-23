target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/memcpy.S
    ${CMAKE_CURRENT_LIST_DIR}/memset.S
    ${CMAKE_CURRENT_LIST_DIR}/setjmp.S
    ${CMAKE_CURRENT_LIST_DIR}/x86_64mach.h
)
