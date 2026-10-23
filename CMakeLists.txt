zephyr_library_named(hg_can_definitions)

zephyr_include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

zephyr_library_include_directories(
    ${CMAKE_CURRENT_SOURCE_DIR}/include/hydrogreen/can
)

zephyr_library_sources(
    src/candef.c
)
