cmake_minimum_required(VERSION 2.8)
project( algoart )
set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 " )
find_package( OpenCV REQUIRED )
add_executable( algoart main.cpp isothetic.cpp)
target_link_libraries( algoart ${OpenCV_LIBS} )