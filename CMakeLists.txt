cmake_minimum_required(VERSION 3.5)

project(learnQtQuick LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)


find_package(Qt5 COMPONENTS Core Quick REQUIRED)

add_subdirectory(src)

#target_compile_definitions(learnQtQuick
#  PRIVATE $<$<OR:$<CONFIG:Debug>,$<CONFIG:RelWithDebInfo>>:QT_QML_DEBUG>)
#target_link_libraries(learnQtQuick
#  PRIVATE Qt5::Core Qt5::Quick)

