cmake_minimum_required(VERSION 2.6)
project(GEP)

add_library (gep
src/geppo/dummy.cpp
)
target_link_libraries(gep SDL2 opengl32 glew32)

add_executable(game
src/game/main.cpp
)

target_link_libraries(game GEP)