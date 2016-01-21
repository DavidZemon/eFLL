set(MODEL cmm)

include_directories("${PROJECT_SOURCE_DIR}")

create_executable(general_simple_sample
    general_simple_sample/general_simple_sample.cpp)
target_link_libraries(general_simple_sample
    eFFL_${MODEL})

create_executable(general_advanced_sample
    general_advanced_sample/general_advanced_sample.cpp)
target_link_libraries(general_advanced_sample
    eFFL_${MODEL})

create_executable(arduino_simple_sample
    arduino_simple_sample/arduino_simple_sample.cpp)
target_link_libraries(arduino_simple_sample
    eFFL_${MODEL})

