cmake_minimum_required(VERSION 3.15)

project(ShFMupL LANGUAGES CXX)

file(TOUCH ${CMAKE_CURRENT_BINARY_DIR}/compile_commands.json)

configure_file(
  ${CMAKE_CURRENT_BINARY_DIR}/compile_commands.json
  ${CMAKE_CURRENT_SOURCE_DIR}/compile_commands.json
  COPYONLY)

option(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_subdirectory(src)
