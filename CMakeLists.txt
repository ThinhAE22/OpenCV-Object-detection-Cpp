cmake_minimum_required(VERSION 3.10)
project(cpp-yolo-detection) # your folder name here

# Find OpenCV
set(OpenCV_DIR C:/OpenCV/opencv/build) # path to opencv
find_package(OpenCV REQUIRED)

add_executable(object-detection object-detection.cpp) # your file name

# Link OpenCV libraries
target_link_libraries(object-detection ${OpenCV_LIBS})