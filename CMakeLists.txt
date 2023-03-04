cmake_minimum_required(VERSION 3.5)

set(FastLED_COMPONENT_SRC_DIRS
    ${CMAKE_CURRENT_LIST_DIR}/src
    ${CMAKE_CURRENT_LIST_DIR}/src/platforms/esp/32
)

set(FastLED_COMPONENT_INCLUDE_DIRS
    ${CMAKE_CURRENT_LIST_DIR}/src
    ${CMAKE_CURRENT_LIST_DIR}/src/platforms/esp/32
)

idf_component_register(SRC_DIRS ${FastLED_COMPONENT_SRC_DIRS}
                       INCLUDE_DIRS ${FastLED_COMPONENT_INCLUDE_DIRS}
                       REQUIRES arduino)

project(FastLED)