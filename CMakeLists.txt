# define the needed version of cmake tool
cmake_minimum_required(VERSION 3.10)

# define the project name
project(summer)

configure_file(${CMAKE_SOURCE_DIR}/main.cpp.in ${CMAKE_BINARY_DIR}/main.cpp @ONLY)
add_executable(${PROJECT_NAME} ${CMAKE_BINARY_DIR}/main.cpp)
