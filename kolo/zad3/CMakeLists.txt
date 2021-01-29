cmake_minimum_required(VERSION 3.10)
project(myProgram)
include_directories(include)
add_executable(myProgram src/Student.cpp)
add_library(libtest STATIC src/libtest.cpp)
target_link_libraries(myProgram libtest)


install(TARGETS libtest DESTINATION ${CMAKE_BINARY_DIR}/../lib)
install(TARGETS myProgram DESTINATION ${CMAKE_BINARY_DIR}/../bin)
