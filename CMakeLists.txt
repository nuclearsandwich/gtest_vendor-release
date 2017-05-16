cmake_minimum_required(VERSION 3.5)

project(gtest_vendor NONE)

install(
  DIRECTORY cmake
  DESTINATION share/${PROJECT_NAME}
)
install(
  FILES package.xml
  DESTINATION share/${PROJECT_NAME}
)
install(
  DIRECTORY vendor/
  DESTINATION src/${PROJECT_NAME}
)
