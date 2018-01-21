cmake_minimum_required(VERSION 2.8)
project(SoundStageNative C CXX)
set(CMAKE_POSITION_INDEPENDENT_CODE ON)
include_directories(${CMAKE_CURRENT_LIST_DIR})

add_library(SoundStageNative SHARED main.cpp Filter.cpp)
set_target_properties(SoundStageNative PROPERTIES LIBRARY_OUTPUT_DIRECTORY ${CMAKE_CURRENT_LIST_DIR}/x64/Release)
