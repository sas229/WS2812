# WS2812 interface library build.
add_library(WS2812 INTERFACE)
target_sources(WS2812 INTERFACE ${CMAKE_CURRENT_LIST_DIR}/src/WS2812.cpp)
target_include_directories(WS2812 INTERFACE ${CMAKE_CURRENT_LIST_DIR}/include/)
target_link_libraries(WS2812 INTERFACE hardware_pio)