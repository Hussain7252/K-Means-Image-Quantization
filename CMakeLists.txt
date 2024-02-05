cmake_minimum_required(VERSION 2.8)
project( KMeans_Clustering )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )

add_executable(colors src/colors.cpp include/kmeans.h src/kmeans.cpp)

target_link_libraries(colors ${OpenCV_LIBS} )
