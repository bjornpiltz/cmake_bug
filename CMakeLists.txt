cmake_minimum_required(VERSION 3.0)

add_subdirectory(lib)

add_executable(app main.cpp)
target_link_libraries(app lib)

#FIND_PACKAGE(Qt5 REQUIRED Core)
#target_link_libraries(app Qt5::Core)