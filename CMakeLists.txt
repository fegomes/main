cmake_minimum_required(VERSION 3.0)
project(main)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${main_SOURCE_DIR}/bin)

include_directories(third_party)

add_subdirectory(third_party)

link_directories(third_party/libhello/lib)

add_executable(main main.cpp main.cpp)

target_link_libraries(main hello)
