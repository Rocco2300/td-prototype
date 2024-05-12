cmake_minimum_required(VERSION 3.23)

project(td-prototype)

include_directories(${CMAKE_SOURCE_DIR}/external/raylib/src)

add_executable(${PROJECT_NAME} main.cpp)

add_subdirectory(${CMAKE_SOURCE_DIR}/external/raylib)

target_link_libraries(${PROJECT_NAME} raylib)
