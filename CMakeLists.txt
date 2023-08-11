cmake_minimum_required(VERSION 3.27.1)
project(sparseOpticalFlow VERSION 0.1.0)

include(CTest)
enable_testing()

set(OpenCV_DIR "C:/opencvOLD/opencv/build/x64/vc15/lib/")   #[[May have to edit this line if opencv is installed at a different location]]
find_package( OpenCV REQUIRED )
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(sparseOpticalFlow main.cpp)

target_link_libraries( sparseOpticalFlow ${OpenCV_LIBS})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)