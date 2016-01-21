cmake_minimum_required(VERSION 3.3)
find_package(PropWare REQUIRED)

project(eFFL)

add_subdirectory(models)
add_subdirectory(examples)

file(GLOB HEADERS *.h)
install(FILES ${HEADERS}
    DESTINATION eFFL/include)

include(CMakeCPack.cmake)
