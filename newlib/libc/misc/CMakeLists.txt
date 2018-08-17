target_sources(c PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/__dprintf.c
    ${CMAKE_CURRENT_LIST_DIR}/ffs.c
    ${CMAKE_CURRENT_LIST_DIR}/fini.c
    ${CMAKE_CURRENT_LIST_DIR}/init.c
    ${CMAKE_CURRENT_LIST_DIR}/lock.c
    ${CMAKE_CURRENT_LIST_DIR}/unctrl.c
)
