set( TARGET src )

set( SOURCE_FILES ./main.cpp )

add_executable( ${TARGET} ${SOURCE_FILES} )

target_link_libraries( ${TARGET}
    impl
)