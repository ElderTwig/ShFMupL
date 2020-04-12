set(CMAKE_CXX_STANDARD 17)

file(GLOB
  SRC
  *.cpp
  *.hpp)

add_executable(game ${SRC})

