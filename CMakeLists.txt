cmake_minimum_required(VERSION 3.5)

project (test)

set(CMAKE_CXX_STANDARD 11)
set(BUILD_DIR   ${CMAKE_BINARY_DIR})

# Instruct CMake to run moc automatically when needed.
set(CMAKE_AUTOMOC ON)

file(GLOB MY_HEADRES "*.h")
file(GLOB MY_SOURCES "*.cpp")

add_executable(testQt ${MY_HEADERS} ${MY_SOURCES})
