cmake_minimum_required(VERSION 3.0)
project(UPS_server)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -pthread")
set(CMAKE_CXX_COMPILER "/usr/bin/g++")

set(SOURCE_FILES main.cpp server.cpp server.h msgTable.cpp msgTable.h gameRoom.cpp gameRoom.h players.h messenger.cpp messenger.h)
add_executable(UPS_server ${SOURCE_FILES})