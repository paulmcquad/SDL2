cmake_minimum_required(VERSION 3.30)
project(sdl-11)

# Debugging Settings (uncomment) :
add_compile_options(-Werror -Wall -Wextra -Wpedantic)

# Set C++ 23 Support
set(CMAKE_CXX_STANDARD 23)

#add_executable(main main.cpp main.hpp input.hpp player.hpp)
add_executable(color_modulation color_modulation.cpp)
target_link_libraries(color_modulation SDL2 SDL2_image)

# Building on Windows with CMake and MinGW
# Run on (cmd)
#
# mkdir build
# cd build
# cmake .. -G "MinGW Makefiles"
# mingw32-make
