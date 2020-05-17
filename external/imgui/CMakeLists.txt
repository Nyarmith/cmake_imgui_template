# collect all .cpp files
file(GLOB imgui_SRCS "*.cpp")
add_library(imgui INTERFACE)
target_include_directories(imgui SYSTEM INTERFACE ${CMAKE_CURRENT_LIST_DIR})
target_sources(imgui INTERFACE ${imgui_SRCS})
