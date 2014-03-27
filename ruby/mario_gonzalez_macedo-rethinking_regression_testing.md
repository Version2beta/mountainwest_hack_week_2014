# Rethinking regression testing

Mario Gonzalez Macedo, @maramono

Average Ruby project: 85% code coverage, 25% test redundancy, 55% regression testing

code coverage is a metric at a point in time.

Mutation score: Ratio (actually, probability)
    * 0 - 100% probability of detection a regression

Mutation analysis:
    * mutate existing source code
    * does a test fail? (has the mute been killed?)

Mutation score is the number of mutants killed over total mutants

competent programmer hypothesis: mostly good, small syntatic erros

first order mutant has one mutation
higher order mutants have more than one.

Libraries

* Ruby Heckle
* Rubant mutant

