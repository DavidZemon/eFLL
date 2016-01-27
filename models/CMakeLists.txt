set(EFFL_SOURCES
    ${PROJECT_SOURCE_DIR}/Fuzzy
    ${PROJECT_SOURCE_DIR}/FuzzyComposition
    ${PROJECT_SOURCE_DIR}/FuzzyInput
    ${PROJECT_SOURCE_DIR}/FuzzyIO
    ${PROJECT_SOURCE_DIR}/FuzzyOutput
    ${PROJECT_SOURCE_DIR}/FuzzyRule
    ${PROJECT_SOURCE_DIR}/FuzzyRuleAntecedent
    ${PROJECT_SOURCE_DIR}/FuzzyRuleConsequent
    ${PROJECT_SOURCE_DIR}/FuzzySet)

add_subdirectory(cog)
add_subdirectory(cmm)
add_subdirectory(lmm)
add_subdirectory(xmm-single)
add_subdirectory(xmm-split)
add_subdirectory(xmmc)
