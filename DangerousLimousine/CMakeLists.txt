cmake_minimum_required(VERSION 3.3)
project(DangerousLimousine)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(BackpackStreaming_SOURCES BackpackStreaming/TestClass.cpp BackpackStreaming/TestClass.h)
add_library(BackpackStreaming ${BackpackStreaming_SOURCES})

set(SOURCE_FILES main.cpp)
add_executable(DangerousLimousine ${SOURCE_FILES} BackpackStreaming)