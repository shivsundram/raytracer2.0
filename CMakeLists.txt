cmake_minimum_required(VERSION 2.8.4)
project(Raytracer1)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -O3 -fopenmp")

include_directories ("${PROJECT_SOURCE_DIR}/eigen")
include_directories ("${PROJECT_SOURCE_DIR}")

set(SOURCE_FILES main.cpp lodepng.cpp)
add_executable(Raytracer1 ${SOURCE_FILES})
target_link_libraries(Raytracer1 ${EXTRA_LIBS})
