cmake_minimum_required(VERSION 3.16)
project(Breakout)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Include headers if you have any
include_directories(src)

# Automatically gather all .cpp and .h files
file(GLOB_RECURSE SOURCES
    src/*.cpp
    src/*.h
)

# Create the executable
add_executable(${PROJECT_NAME} ${SOURCES})