add_executable(compressor-benchmark main.cpp)
target_include_directories(compressor-benchmark PRIVATE .. PRIVATE $<TARGET_PROPERTY:CONAN_PKG::imgui,INTERFACE_INCLUDE_DIRECTORIES>)
target_link_libraries(compressor-benchmark PRIVATE CONAN_PKG::imgui imgui-ws)
