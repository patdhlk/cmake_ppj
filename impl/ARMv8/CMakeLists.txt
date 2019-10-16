set( TARGET impl )

set( SOURCE_FILES 
    Bob.cpp
)

add_library( ${TARGET} ${SOURCE_FILES} )

target_include_directories( ${TARGET}
	PUBLIC
		${CMAKE_CURRENT_SOURCE_DIR}
)