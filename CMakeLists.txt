add_library(LodePNG STATIC
    lodepng.cpp
)
target_include_directories(LodePNG
    PUBLIC
        .
)
set_target_properties(LodePNG PROPERTIES
    LINKER_LANGUAGE CXX
)
add_library(LodePNG::LodePNG ALIAS LodePNG)