cmake_minimum_required(VERSION 3.0.0)

project(lab)

file(GLOB codeFiles *.cpp)

set(CMAKE_CXX_STANDARD, 17)
set(CMAKE_CXX_FLAGS, "${CMAKE_CXX_FLAGS} -g -Wall -Wextra")

# place executable in /bin directory
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)

add_executable(lab ${codeFiles})

