add_executable(freebot-realtime freebot-realtime.cpp freebot_arm_ik_control.cpp freebot_base_control.cpp)
target_link_libraries(freebot-realtime rt ${RBDL_LIBRARY} ${RBDL_URDFReader_LIBRARY} yaml-cpp motor_manager)
target_include_directories(freebot-realtime PUBLIC ../include ${RBDL_PATH}/include ${EIGEN3_INCLUDE_DIR})
