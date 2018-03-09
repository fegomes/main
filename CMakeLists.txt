cmake_minimum_required(VERSION 3.0)
project(main)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${main_SOURCE_DIR}/bin)

add_subdirectory(third_party)

add_executable(main main.cpp main.cpp)

