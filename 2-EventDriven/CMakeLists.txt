cmake_minimum_required(VERSION 3.30)
project(sdl-2)

# Debugging Settings (uncomment) :
add_compile_options(-Werror -Wall -Wextra -Wpedantic)

# Set C++ 23 Support
set(CMAKE_CXX_STANDARD 23)

#add_executable(main main.cpp main.hpp input.hpp player.hpp)
add_executable(event_driven event_driven.cpp)
target_link_libraries(event_driven SDL2)

# Building on Windows with CMake and MinGW
# Run on (cmd)
#
# mkdir build
# cd build
# cmake .. -G "MinGW Makefiles"
# mingw32-make
