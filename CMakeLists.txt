cmake_minimum_required(VERSION 3.10)
project(SFMLApp)

# Find SFML package
find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

# Add your source files
set(SOURCES main.cpp)

# Create executable
add_executable(sfml-app ${SOURCES})

# Link SFML libraries
target_link_libraries(sfml-app PRIVATE sfml-graphics sfml-window sfml-system)
