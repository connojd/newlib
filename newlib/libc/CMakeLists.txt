# Copyright (C) 2018 Connor Davis
#
# Permission to use, copy, modify, and distribute this software
# is freely granted, provided that this notice is preserved.
#

add_library(c)

target_compile_features(c PRIVATE c_std_11)
target_include_directories(c PRIVATE
    $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/include>
    $<BUILD_INTERFACE:${TARG_INC}>
    $<INSTALL_INTERFACE:include>
)

#add_subdirectory(argz)
#add_subdirectory(ctype)
#add_subdirectory(errno)
#add_subdirectory(locale)
#add_subdirectory(machine/x86_64)
#add_subdirectory(misc)
#add_subdirectory(reent)
#add_subdirectory(search)
#add_subdirectory(signal)
#add_subdirectory(ssp)
#add_subdirectory(stdio)
#add_subdirectory(stdlib)
#add_subdirectory(string)
#add_subdirectory(time)

#install(TARGETS c DESTINATION lib)
#install(DIRECTORY ${CMAKE_CURRENT_LIST_DIR}/include/ DESTINATION include)
