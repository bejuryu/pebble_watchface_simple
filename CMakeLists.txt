cmake_minimum_required(VERSION 3.3)
project(watchface_simple)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES src/c/watchface_simple.c)

include_directories(
        "~/.pebble-sdk/SDKs/current/sdk-core/pebble/basalt/include"
        "./build/basalt/src"
)
add_executable(${PROJECT_NAME} ${SOURCE_FILES})