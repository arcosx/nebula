# Copyright (c) 2020 vesoft inc. All rights reserved.
#
# This source code is licensed under Apache 2.0 License.

nebula_add_test(
    NAME
        concurrent_test
    SOURCES
        BarrierTest.cpp LatchTest.cpp
    OBJECTS
        $<TARGET_OBJECTS:concurrent_obj>
        $<TARGET_OBJECTS:thread_obj>
        $<TARGET_OBJECTS:time_obj>
    LIBRARIES
        gtest
        gtest_main
)
