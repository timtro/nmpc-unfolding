add_executable(catnav2)
target_sources(
  catnav2
  PRIVATE catnav2.cpp
  INTERFACE ../include/nmpc_algebra.hpp ../include/XY.hpp
            ../include/nav2_Pose.hpp)

target_link_libraries(catnav2 PRIVATE project_warnings project_options
                                      Nav2remote Obstacle JsonNMPCLogger)
