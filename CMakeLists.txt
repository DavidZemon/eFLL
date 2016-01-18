cmake_minimum_required(VERSION 3.3)
find_package(PropWare REQUIRED)

project(eFFL)

set(MODEL lmm)
set_compile_flags()
add_library(eFFL
    Fuzzy
    FuzzyComposition
    FuzzyInput
    FuzzyIO
    FuzzyOutput
    FuzzyRule
    FuzzyRuleAntecedent
    FuzzyRuleConsequent
    FuzzySet)

add_subdirectory(examples)
