##
 #  Explain       :     CMake configuraiton for Data Structures in C++ Repository 
 #  Author        :     Mehmet Ekemen
 #  Nickname      :     `hun
 #  Email         :     ekemenms@hotmail.com
 #  Date          :     16.10.2020
 #  Github        :     github.com/hun756   
 #  Resource      :     https://github.com/hun756/Data-Sutructures-in-CPlusPlus/
##

# Set minimum CMake version.
cmake_minimum_required(VERSION 2.8)

# Name the project.
project(Data_Sutructures_in_Cpp)

# Set project directory instead of CMAKE_SORUCE_DIR
set(PROJECT_DIR ${CMAKE_SOURCE_DIR})

# Set project include directory.
set(PROJECT_INCLUDE_DIR ${PROJECT_DIR}/include)

# Set projects resources directory.
set(PROJECT_RESOURCES_DIR ${PROJECT_DIR}/resources)

# Project resources content.
set(PROJECT_RESOURCES
        # ${PROJECT_RESOURCES_DIR}/my_class.cpp
        ${PROJECT_RESOURCES_DIR}/main.cpp
   )

# Include header filesç.
include_directories(${PROJECT_INCLUDE_DIR})

# Executable.
add_executable(${PROJECT_NAME} ${PROJECT_RESOURCES})
