include(p.cmake)

if ( DEFINED IMPL_DIR AND EXISTS ${CMAKE_SOURCE_DIR}/impl/${IMPL_DIR} )
    add_subdirectory( ${IMPL_DIR} )
else ()
    message( FATAL_ERROR "error" )
endif()