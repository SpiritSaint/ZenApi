cmake_minimum_required(VERSION 3.16)
project(ZenAPI)

set(CMAKE_CXX_STANDARD 11)
find_package(Boost 1.78 COMPONENTS regex json REQUIRED)
include_directories( ${Boost_INCLUDE_DIR} )

add_executable(ZenAPI main.cpp)
SET(CMAKE_CXX_FLAGS "-pthread")