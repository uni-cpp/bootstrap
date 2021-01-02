cmake_minimum_required( VERSION 3.10 )

project( uni )

include( ${CMAKE_SOURCE_DIR}/cmake/bootstrap.cmake )

set( SOURCE_DIR "${CMAKE_SOURCE_DIR}" )
set( BUILD_DIR "${CMAKE_BINARY_DIR}" )
set( INSTALL_DIR "${BUILD_DIR}/install" )

set( CMAKE_INSTALL_PREFIX ${INSTALL_DIR} )
set( CMAKE_INSTALL_RPATH ${INSTALL_DIR}/usr/lib )
set( CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE )

add_subdirectory( ${SOURCE_DIR}/common )
add_subdirectory( ${SOURCE_DIR}/async-data-manager )
add_subdirectory( ${SOURCE_DIR}/san-issue-detector )
add_subdirectory( ${SOURCE_DIR}/motors )
