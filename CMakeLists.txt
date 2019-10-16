# CMake version
cmake_minimum_required(VERSION 3.0)

# Meta information about the project
set(META_PROJECT_NAME        "Awesome")
set(META_PROJECT_DESCRIPTION "Whatever")

project(${META_PROJECT_NAME} C CXX)

# set some additional module path
SET( CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${PROJECT_SOURCE_DIR}/ppj_cmake_modules )

# set a variable for the implementation, set the CPU model
# changing this variable requires to regenerate the project/makefiles
set( CPU_M "ARMv8")

# include variations 
include( impl ) # defined in ppj_cmake_modules/impl.cmake

# directory with the source code
add_subdirectory( src )