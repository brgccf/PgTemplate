cmake_minimum_required(VERSION 2.8)
project(ProjetoPg)
find_package(OpenGL REQUIRED)
find_package(X11)
include_directories(glfw/include ${OPENGL_INCLUDE_DIRS})
add_subdirectory(glfw)
add_executable(ProjetoPg template.cpp)
target_link_libraries(ProjetoPg glfw  ${OPENGL_LIBRARIES} ${GLFW_LIBRARIES})
#created by alpgc
