file( GLOB SRC *.cpp )
file( GLOB HDR *.h )
#
add_library( library PRIVATE  ${SRC} ${HDR} )
