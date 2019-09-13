cmake_minimum_required(VERSION 3.1)
project(hello)

message(STATUS "binary dir: ${PROJECT_BINARY_DIR}")
message(STATUS "source dir:" ${PROJECT_SOURCE_DIR})

add_executable(hello main.c)