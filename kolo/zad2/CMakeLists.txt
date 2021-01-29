cmake_minimum_required(VERSION 3.10)
project(myProgram)
include(address.h)
include(employee.h)
add_executable(myProgram main.cpp employee.cpp address.cpp)

