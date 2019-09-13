cmake_minimum_required(VERSION 3.1)
project(boost_demo)

find_package(Boost REQUIRED)

add_executable(boost_demo main.cpp)
target_link_libraries(boost_demo ${Boost_LIBRARIES})
