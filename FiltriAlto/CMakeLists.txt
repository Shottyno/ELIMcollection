cmake_minimum_required(VERSION 2.8)
project( alto )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( alto alto.cpp )
target_link_libraries( alto ${OpenCV_LIBS} )