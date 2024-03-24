add_subdirectory (AircraftHud)

add_subdirectory (SkyboltCommon)
add_subdirectory (SkyboltCommonTests)

add_subdirectory (SkyboltSim)
add_subdirectory (SkyboltSimTests)

add_subdirectory (SkyboltVis)
add_subdirectory (SkyboltVisTests)

add_subdirectory (SkyboltEngine)
add_subdirectory (SkyboltEngineTests)

OPTION(BUILD_PYTHON_BINDINGS "Build Python Bindings")
if (BUILD_PYTHON_BINDINGS)
	add_subdirectory (SkyboltEnginePython)
endif()

add_subdirectory (SkyboltEnginePlugins)

add_subdirectory (TileMapGenerator)
OPTION(BUILD_MAP_FEATURES_CONVERTER "Build MapFeaturesConverter")
if (BUILD_MAP_FEATURES_CONVERTER)
	#add_subdirectory (MapFeaturesConverter)
endif()