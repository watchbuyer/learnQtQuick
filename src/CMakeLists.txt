
find_package(Qt5 COMPONENTS Core Quick REQUIRED)

set(HEADERS

)

set(SOURCES
main.cpp

)

add_executable(${PROJECT_NAME} ${HEADERS} ${SOURCES} "qml.qrc" "main.qml")  

#target_compile_definitions(learnQtQuick
#  PRIVATE $<$<OR:$<CONFIG:Debug>,$<CONFIG:RelWithDebInfo>>:QT_QML_DEBUG>)
#target_link_libraries(learnQtQuick
#  PRIVATE Qt5::Core Qt5::Quick)

target_compile_definitions(learnQtQuick
  PRIVATE $<$<OR:$<CONFIG:Debug>,$<CONFIG:RelWithDebInfo>>:QT_QML_DEBUG>)
target_link_libraries(learnQtQuick
  PRIVATE Qt5::Core Qt5::Quick)