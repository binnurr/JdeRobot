add_library (pioneer STATIC pioneer.c pioneer.h)

add_library (pioneershare SHARED pioneer.c pioneer.h)

set_target_properties(pioneershare PROPERTIES OUTPUT_NAME pioneer)

### Install
install(TARGETS pioneer pioneershare
    DESTINATION ${CMAKE_INSTALL_PREFIX}/lib/jderobot
    COMPONENT core
)
