cmake_minimum_required(VERSION 3.10)
project(SFMLExample)

set(CMAKE_CXX_STANDARD 17)

# Set path to SFML directory
set(SFML_ROOT "${CMAKE_SOURCE_DIR}/SFML")

# Add SFML include and lib directories
include_directories("${SFML_ROOT}/include")
link_directories("${SFML_ROOT}/lib")

add_executable(play main.cpp)

target_link_libraries(play sfml-graphics sfml-window sfml-system sfml-audio)

