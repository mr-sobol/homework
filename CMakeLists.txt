cmake_minimum_required(VERSION 3.5)

project(homework VERSION 0.0.1$ENV{TRAVIS_BUILD_NUMBER})

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Threads REQUIRED)

add_executable(homework
  main.cpp
)
target_link_libraries(homework Threads::Threads)
