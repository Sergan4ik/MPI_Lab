cmake_minimum_required(VERSION 3.27)
project(PMSort)

set(CMAKE_CXX_STANDARD 17)

find_package(MPI REQUIRED)

add_executable(PMSort main.cpp)

target_link_libraries(PMSort PRIVATE MPI::MPI_CXX)