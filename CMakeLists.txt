cmake_minimum_required(VERSION 3.23)
project(PokeExpansion C)

set(CMAKE_C_STANDARD 11)

include_directories(src)
include_directories(src/defines)
ADD_DEFINITIONS(-D__INTELLISENSE__)

add_executable(PokeExpansion
        src/defines/pokes.h
        src/defines.h
        src/DexExpansion.c
        src/functions.h
        src/locations.h
        src/Saveblock.c
        src/structs.h
        src/types.h src/species_name.c src/base_stats.c src/dex.c)
