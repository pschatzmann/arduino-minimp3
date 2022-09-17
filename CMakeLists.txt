cmake_minimum_required(VERSION 3.16)

# set the project name
project(arduino_minimp3)

# lots of warnings and all warnings as errors
## add_compile_options(-Wall -Wextra )
set(CMAKE_CXX_STANDARD 17)

# define libraries
add_library (arduino_minimp3 INTERFACE)

# define location for header files
target_include_directories(arduino_minimp3 INTERFACE ${CMAKE_CURRENT_SOURCE_DIR} )
