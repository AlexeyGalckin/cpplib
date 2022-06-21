file( GLOB SRC *.cpp )
file( GLOB HDR *.hpp )
#
add_executable( library ${SRC} ${HDR})
#
target_link_libraries( library-test PRIVATE library GTest::gtest GTest::gtest_main )
#
gtest_add_tests(TARGET library-test )
