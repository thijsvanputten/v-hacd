cmake_minimum_required(VERSION 3.0.0 FATAL_ERROR)
project(VHACD)
option(NO_OPENCL "NO_OPENCL" OFF)
option(NO_OPENMP "NO_OPENMP" OFF)

message("NO_OPENCL " ${NO_OPENCL})
message("NO_OPENMP " ${NO_OPENMP})

set(CMAKE_INSTALL_PREFIX "${CMAKE_SOURCE_DIR}/../install" CACHE PATH "project install prefix" FORCE)
set(CMAKE_COMMON_INC "${CMAKE_SOURCE_DIR}/../scripts/cmake_common.cmake")
add_subdirectory ("${CMAKE_SOURCE_DIR}/VHACD_Lib")
#add_subdirectory ("${CMAKE_SOURCE_DIR}/test")
