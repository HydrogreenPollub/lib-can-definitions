zephyr_library_named(hg_can_definitions)

set(can_public_include_dir "${CMAKE_CURRENT_BINARY_DIR}/include")
configure_file("${CMAKE_CURRENT_SOURCE_DIR}/candef.h"
               "${can_public_include_dir}/hydrogreen/can/candef.h" COPYONLY)
zephyr_include_directories("${can_public_include_dir}")
zephyr_library_sources(candef.c)
