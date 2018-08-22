cmake_minimum_required(VERSION 3.6.0)
project(newlib VERSION 3.0.0 LANGUAGES C)

#
# Module includes
#
include(CMakePackageConfigHelpers)

#
# EXPORT_DIR
#
# Path to install target exports and cmake config files.
# This must be relative to the install prefix. Note that it
# must always be set to a directory searched for by find_package.
#
set(EXPORT_DIR lib/cmake)

configure_package_config_file(
    newlib-config.cmake.in
    newlib-config.cmake
    INSTALL_DESTINATION "${EXPORT_DIR}/newlib"
    PATH_VARS EXPORT_DIR
    NO_SET_AND_CHECK_MACRO
    NO_CHECK_REQUIRED_COMPONENTS_MACRO
)

install(
    FILES ${CMAKE_CURRENT_BINARY_DIR}/newlib-config.cmake
    DESTINATION "${EXPORT_DIR}/newlib"
)

install(
    EXPORT newlib::lib
    DESTINATION "${EXPORT_DIR}/newlib"
    NAMESPACE newlib::lib
    FILE newlib-targets.cmake
)

add_subdirectory(newlib)











