cmake_minimum_required(VERSION 3.18)

project(Stack)

set(STACK_DIR ${CMAKE_CURRENT_SOURCE_DIR}/stack)
set(STACK_INCLUDE_DIR ${STACK_DIR}/include)
message("STACK_DIR = ${STACK_DIR}")
message("STACK_INCLUDE_DIR = ${STACK_INCLUDE_DIR}")

add_subdirectory(stack)
add_subdirectory(googletest)

include_directories(${STACK_INCLUDE_DIR})

add_executable(main main.cpp)
target_link_libraries(main stack)

add_executable(tests tests.cpp)
target_link_libraries(tests stack gtest gtest_main)
