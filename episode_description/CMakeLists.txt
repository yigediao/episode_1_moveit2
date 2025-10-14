cmake_minimum_required(VERSION 3.8)
project(episode_description)

find_package(ament_cmake REQUIRED)

# 没有要编译的源码，只安装资源目录到 share/episode_description 下
install(DIRECTORY
  urdf
  meshes
  config
  launch
  include
  DESTINATION share/${PROJECT_NAME}
)

ament_package()
