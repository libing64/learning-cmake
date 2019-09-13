cmake_minimum_required(VERSION 3.1)

message(STATUS "1. executable output path: ${EXECUTABLE_OUTPUT_PATH}")
message(STATUS "1. library output path: ${EXECUTABLE_OUTPUT_PATH}")
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib)
message(STATUS "2. executable output path: ${EXECUTABLE_OUTPUT_PATH}")
message(STATUS "2. library output path: ${EXECUTABLE_OUTPUT_PATH}")
add_executable(hello main.c)

install(FILES COPYRIGHT README.md DESTINATION share/doc/make/hello-world-clear)
install(PROGRAMS runhello.sh DESTINATION bin)


