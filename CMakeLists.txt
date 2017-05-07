cmake_minimum_required(VERSION 3.7)
project(thread)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES main.cpp)

find_package(Threads)

add_executable(thread ${SOURCE_FILES})
target_link_libraries(thread ${CMAKE_THREAD_LIBS_INIT})