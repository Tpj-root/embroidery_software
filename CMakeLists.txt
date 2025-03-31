cmake_minimum_required(VERSION 3.10)
project(EmbroiderySoftware)

set(CMAKE_CXX_STANDARD 17)

# Add source files
add_executable(embroidery_software 
    embroidery_software.cpp 
)

# Include header files
target_include_directories(embroidery_software PRIVATE ${CMAKE_SOURCE_DIR})

# Link necessary libraries (if needed)
# target_link_libraries(embroidery_software some_library)

# Ensure standard system libraries are included
target_link_libraries(embroidery_software PRIVATE stdc++)
