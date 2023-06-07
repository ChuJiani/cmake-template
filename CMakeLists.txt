cmake_minimum_required(VERSION 3.8)

# Global Config
if (NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release)
endif()

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# Root Project
project(demo 
    LANGUAGES CXX
    VERSION 0.1.0
    DESCRIPTION "Some description"
    HOMEPAGE_URL "Some website"
    )

# Project Config
# set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)
# set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)

# Global-Used 3rd Party Libraries
# include_directories(///include/eigen3)

# Subprojects
add_subdirectory(sub1) 

