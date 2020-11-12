add_executable(basic-null main.cpp)
target_include_directories(basic-null PRIVATE .. PRIVATE $<TARGET_PROPERTY:CONAN_PKG::imgui,INTERFACE_INCLUDE_DIRECTORIES>)
target_link_libraries(basic-null PRIVATE CONAN_PKG::imgui imgui-ws)
