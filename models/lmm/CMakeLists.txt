set(MODEL lmm)
set_compile_flags()
add_library(eFFL_${MODEL} ${EFFL_SOURCES})
set_target_properties(eFFL_${MODEL} PROPERTIES OUTPUT_NAME eFFL)
install(TARGETS eFFL_${MODEL}
    DESTINATION eFFL/lib/${MODEL}
    EXPORT eFFL-targets)
