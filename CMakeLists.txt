cmake_minimum_required(VERSION 3.19)
project(libbech32_client)

set(CMAKE_CXX_STANDARD 11)

find_package(libbech32 1.0.1 REQUIRED)

add_executable(libbech32_client main.cpp)

target_link_libraries(libbech32_client bech32::bech32)
