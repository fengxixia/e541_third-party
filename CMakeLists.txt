cmake_minimum_required(VERSION 3.15)
project(curl NONE)

# 安装头文件
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/
        DESTINATION usr/include
        FILES_MATCHING PATTERN "*.h")

# 安装库文件
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/lib/
        DESTINATION usr/lib)

# 可选：安装 curlConfig.cmake
# install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/cmake/
#         DESTINATION lib/cmake/curl)
