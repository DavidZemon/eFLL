set(MODEL xmm-split)
set_compile_flags()
add_library(eFFL_${MODEL}
    ${PROJECT_SOURCE_DIR}/Fuzzy
    ${PROJECT_SOURCE_DIR}/FuzzyComposition
    ${PROJECT_SOURCE_DIR}/FuzzyInput
    ${PROJECT_SOURCE_DIR}/FuzzyIO
    ${PROJECT_SOURCE_DIR}/FuzzyOutput
    ${PROJECT_SOURCE_DIR}/FuzzyRule
    ${PROJECT_SOURCE_DIR}/FuzzyRuleAntecedent
    ${PROJECT_SOURCE_DIR}/FuzzyRuleConsequent
    ${PROJECT_SOURCE_DIR}/FuzzySet)
set_target_properties(eFFL_${MODEL} PROPERTIES OUTPUT_NAME eFFL)
install(TARGETS eFFL_${MODEL}
    DESTINATION eFFL/lib/${MODEL}
    EXPORT eFFL-targets)
