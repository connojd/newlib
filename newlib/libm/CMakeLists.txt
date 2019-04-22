#
# Copyright (C) 2019 Assured Information Security
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

add_library(m)

target_compile_features(m PRIVATE c_std_11)
target_compile_definitions(m PRIVATE MALLOC_PROVIDED _COMPILING_NEWLIB)
target_compile_definitions(m PRIVATE __NO_SYSCALLS__ MISSING_SYSCALL_NAMES)
target_include_directories(m SYSTEM PRIVATE
    $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/../libc/include>
    $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/common>
    $<INSTALL_INTERFACE:include>
)

add_subdirectory(common)
add_subdirectory(complex)
add_subdirectory(math)

install(TARGETS m DESTINATION lib)
