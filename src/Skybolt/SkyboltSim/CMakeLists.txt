set(LIB_NAME SkyboltSim)

add_source_group_tree(. SOURCE_FILES)

include_directories("../")

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(LIBRARIES
	SkyboltCommon
)

add_library(${LIB_NAME} STATIC ${SOURCE_FILES} ${HEADER_FILES})

target_link_libraries(${LIB_NAME} PUBLIC ${LIBRARIES})

skybolt_install(${LIB_NAME})