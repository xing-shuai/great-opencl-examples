# set minimum cmake version
cmake_minimum_required(VERSION 3.0)
project(OpenCLTEST LANGUAGES C CXX)


message(STATUS ">>>>>>>>>>>>>")
message(STATUS "\tSystem: ${CMAKE_SYSTEM_NAME}")
message(STATUS "\tProcessor: ${CMAKE_SYSTEM_PROCESSOR}")

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -std=gnu99")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14")


add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/print_info)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/hello_world)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/array_addition)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/matrix_multiplication)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/cached_matrix_multiplication)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/image_filtering)