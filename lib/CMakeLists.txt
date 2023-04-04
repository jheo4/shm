set( CMAKE_INCLUDE_CURRENT_DIR ON )

add_library( shm SHARED shm.cpp )

target_link_libraries( shm ${CMAKE_NUMA_LIBS} )
install( TARGETS shm
         ARCHIVE DESTINATION ${CMAKE_INSTALL_PREFIX}/lib )
