add_executable(image_filtering image_filtering.cpp)
target_link_libraries(image_filtering -lOpenCL -lpthread -lm -lX11)