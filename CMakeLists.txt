cmake_minimum_required(VERSION 3.16.3)

project(imgui-cmake LANGUAGES C CXX)

add_subdirectory(lib)

add_executable(example example.cpp)

target_link_libraries(example PRIVATE IMGUI
        d3d11.lib
        dwmapi.lib
        d3dcompiler.lib)




