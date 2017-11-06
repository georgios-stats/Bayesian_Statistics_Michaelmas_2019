---
output:
  pdf_document: default
  html_document: default
---
# Bayesian Statistics

Here is a list of interactive applications related to the course *Bayesian Statistics course Level III/IV* .

To use these applications run *rstudio*, and set your workspace to be *Bayesian_Statistics* .

## Install dependences

> install.packages("rmarkdown")  

## A Biostatistics exmple

This is just an simple Bayesian example from Biostatistics (... and Statistics I)

Execute command

  > rmarkdown::run("./demo_Biostatistics_Bayes/demo_Biostatistics_Bayes.Rmd")

## Known distributions

Just some known distributions

Execute command

  > rmarkdown::run("./demo_distributions/demo_distributions.Rmd")

## Central limit Theorem

A demo about the central limit theorem

Execute command

  > rmarkdown::run("./demo_CLT/demo_CLT.Rmd")

## Weak law of large numbers

A demo about the weak law of large number

Execute command

  > rmarkdown::run("./demo_WLLN/demo_WLLN.Rmd")

## Conjugate priors

Explore the behaviour of the posterior distribution, with respect to the hyperparameters of the prior distributions, and the number of observables. 

Execute command

  > rmarkdown::run("./demo_WLLN/demo_ConjugatePriors.Rmd")





  