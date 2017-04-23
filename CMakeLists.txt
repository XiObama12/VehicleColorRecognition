cmake_minimum_required(VERSION 2.8)
project(VehicleColorRecognition)

set(CMAKE_BUILD_TYPE Debug)
set(OpenCV_DIR "/usr/include")
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
add_executable(ColorRecognition main.cpp)
target_link_libraries(ColorRecognition ${OpenCV_LIBS})
