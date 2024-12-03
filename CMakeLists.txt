cmake_minimum_required(VERSION 3.28)
cmake_minimum_required(VERSION 3.10)
project(untitled1)

find_package(MPI REQUIRED)

include_directories(${MPI_CXX_INCLUDE_PATH})

set(CMAKE_CXX_STANDARD 17)

add_executable(untitled1 main.cpp)

target_link_libraries(untitled1 ${MPI_CXX_LIBRARIES})
