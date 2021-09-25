cmake_minimum_required(VERSION 3.12)

project(simple_lib)

add_library(simple_lib src/simple_lib.cc)

target_include_directories(simple_lib PUBLIC
        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>)