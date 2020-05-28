cmake_minimum_required (VERSION 3.5)
set( prjName UnscentedKF )

add_definitions(-std=c++0x)
add_definitions(-DDEBUG)


###### change the default location of executables
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)


set(sources
   src/ukf.cpp
   src/main.cpp
   src/tools.cpp)

add_executable(${prjName} ${sources})
