cmake_minimum_required(VERSION 3.0)

add_library(lib lib.cpp lib.h)
target_include_directories(lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

FIND_PACKAGE(Qt5 REQUIRED Core)
target_link_libraries(lib Qt5::Core)
