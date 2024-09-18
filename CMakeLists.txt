cmake_minimum_required(VERSION 3.14)

# Set the project name
project(QtHelloWorld VERSION 1.0)

# Find the Qt libraries
set(CMAKE_PREFIX_PATH "C:/Qt/5.15.2/msvc2019_64")
find_package(Qt5 COMPONENTS Widgets REQUIRED)

# Add the executable
add_executable(QtHelloWorld main.cpp)

# Link the Qt libraries
target_link_libraries(QtHelloWorld Qt5::Widgets)
