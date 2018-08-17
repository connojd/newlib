target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/x86_64/memcpy.S
    ${CMAKE_CURRENT_LIST_DIR}/x86_64/memset.S
    ${CMAKE_CURRENT_LIST_DIR}/x86_64/setjmp.S
    ${CMAKE_CURRENT_LIST_DIR}/x86_64/x86_64mach.h
)
