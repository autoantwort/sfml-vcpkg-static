cmake_minimum_required(VERSION 3.20)

project(test VERSION 0.0.1 LANGUAGES CXX)

add_executable(main)
target_sources(main PRIVATE main.cpp)

set_property(TARGET main PROPERTY MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")

find_package(SFML COMPONENTS system window graphics CONFIG REQUIRED)
target_link_libraries(main PRIVATE sfml-system sfml-network sfml-graphics sfml-window)
