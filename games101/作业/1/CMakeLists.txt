cmake_minimum_required(VERSION 3.10)
project(Rasterizer)

find_package(OpenCV REQUIRED)

set(CMAKE_CXX_STANDARD 17)

include_directories(/usr/local/include)

add_executable(Rasterizer main.cc rasterizer.h rasterizer.cc Triangle.h Triangle.cc)
target_link_libraries(Rasterizer ${OpenCV_LIBRARIES})
