cmake_minimum_required(VERSION 3.10)

project(solver_application)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(solver_application equation.cpp)

target_link_libraries(solver_application PRIVATE solver_lib formatter_ex)

target_include_directories(solver_application PRIVATE
    ${CMAKE_SOURCE_DIR}/solver_lib
    ${CMAKE_SOURCE_DIR}/formatter_ex_lib
    ${CMAKE_SOURCE_DIR}/formatter_lib
)
