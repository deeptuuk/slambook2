cmake_minimum_required( VERSION 2.8)

project( gaussNewton )
set( CMAKE_CXX_FLAGS "-std=c++11" )

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )

#find_package( Sophus REQUIRED )
#include_directories( ${Sophus_INCLUDE_DIRS} )

include_directories( "/usr/include/eigen3" )

add_executable( gaussNewton gaussNewton.cpp )
target_link_libraries( gaussNewton ${OpenCV_LIBS} )

