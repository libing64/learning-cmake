cmake_minimum_required(VERSION 3.1)

find_package(CURL REQUIRED)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)


if (CURL_FOUND)
  add_executable(curl_demo main.c)
  target_link_libraries(curl_demo ${CURL_LIBRARY})
else (CURL_FOUND)
  message(FATAL_ERROR "CURL library not found")
endif (CURL_FOUND)