cmake_minimum_required(VERSION 3.0)

project(JetsonFaceDetection)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS} ${PROJECT_SOURCE_DIR})

add_executable(jetsonFaceDetection faceDetection.cpp)

target_link_libraries(jetsonFaceDetection ${OpenCV_LIBS})