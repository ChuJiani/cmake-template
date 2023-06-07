# New executable target
file(GLOB_RECURSE sources CONFIGURE_DEPENDS src/*.cpp include/*.h)
add_executable(sub1 ${sources})
target_include_directories(sub1 PUBLIC include)
