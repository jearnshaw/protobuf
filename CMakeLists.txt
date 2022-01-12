cmake_minimum_required(VERSION 3.2)

include("cmake/HunterGate.cmake")
HunterGate(
    URL "https://github.com/cpp-pm/hunter/archive/v0.23.320.tar.gz"
    SHA1 "9b4e732afd22f40482c11ad6342f7d336634226f"
)

# Project
project(protobuf C CXX)

hunter_add_package(ZLIB)

add_subdirectory(cmake)
