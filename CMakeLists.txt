cmake_minimum_required(VERSION 3.5.0)

project(test)
set(CMAKE_CXX_STANDARD 17)
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
aux_source_directory(${PROJECT_SOURCE_DIR}/ DIR_LISTS)

add_executable(test ${DIR_LISTS})

target_link_libraries(
    test
    PUBLIC
    easyx
)



