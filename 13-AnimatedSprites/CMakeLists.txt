cmake_minimum_required(VERSION 3.30)
project(sdl-13)

# Debugging Settings (uncomment) :
add_compile_options(-Werror -Wall -Wextra -Wpedantic)

# Set C++ 23 Support
set(CMAKE_CXX_STANDARD 23)

#add_executable(main main.cpp main.hpp input.hpp player.hpp)
add_executable(animated_sprites animated_sprites.cpp)
target_link_libraries(animated_sprites SDL2 SDL2_image)

# Building on Windows with CMake and MinGW
# Run on (cmd)
#
# mkdir build
# cd build
# cmake .. -G "MinGW Makefiles"
# mingw32-make
