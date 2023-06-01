cmake_minimum_required(VERSION 3.24)

set(CMAKE_PROJECT_TOP_LEVEL_INCLUDES ../conan_provider.cmake)

project(FormatOutput LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

find_package(fmt REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main PRIVATE fmt::fmt)                    