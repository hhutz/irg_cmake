cmake_minimum_required(VERSION 2.8.3)
project(irg_cmake)

if (${CATKIN_TOPLEVEL})
find_package(catkin)
endif(${CATKIN_TOPLEVEL})


if (catkin_FOUND)
  ###################################
  ## catkin specific configuration ##
  ###################################
  catkin_package(
    CFG_EXTRAS irg_cmake-extras.cmake
  )

  install(DIRECTORY Modules
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/irg_cmake
  )
endif (catkin_FOUND)
