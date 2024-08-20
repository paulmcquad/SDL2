cmake_minimum_required(VERSION 3.30)
project(sdl-15)

# Debugging Settings (uncomment) :
add_compile_options(-Werror -Wall -Wextra -Wpedantic)

# Set C++ 23 Support
set(CMAKE_CXX_STANDARD 23)

#add_executable(main main.cpp main.hpp input.hpp player.hpp)
add_executable(true_type_fonts true_type_fonts.cpp)
target_link_libraries(true_type_fonts SDL2 SDL2_image SDL2_ttf)

# Building on Windows with CMake and MinGW
# Run on (cmd)
#
# mkdir build
# cd build
# cmake .. -G "MinGW Makefiles"
# mingw32-make
