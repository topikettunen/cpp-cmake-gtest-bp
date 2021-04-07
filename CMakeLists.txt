cmake_minimum_required(VERSION 3.19.5)

set(PROJECT project)

project(
  ${PROJECT}
  LANGUAGES CXX
  DESCRIPTION "Project description") 

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}) 

enable_testing()

include_directories(${CMAKE_SOURCE_DIR})

add_subdirectory(${PROJECT})
