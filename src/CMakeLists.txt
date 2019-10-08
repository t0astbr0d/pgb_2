cmake_minimum_required(VERSION 3.1)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)
if(CMAKE_VERSION VERSION_LESS "3.7.0")
	set(CMAKE_INCLUDE_CURRENT_DIR ON)
endif()


project(pgb1)
add_executable(main main.cpp)

find_package(Qt5 COMPONENTS Widgets REQUIRED)
target_link_libraries(main Qt5::Widgets)