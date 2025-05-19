
cmake_minimum_required(VERSION 3.4)

project(hello_world)

add_subdirectory(../formatter_ex_lib build_formatter_ex)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(hello_world hello_world.cpp)

target_link_libraries(hello_world PUBLIC formatter_ex)

