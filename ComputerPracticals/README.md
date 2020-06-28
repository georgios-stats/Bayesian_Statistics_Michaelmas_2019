Aim
===

The handout aims at familiarising students with the statistical package
RJAGS, and with more ‘sophisticated’ Bayesian hierarchical models than
those in the Lecture handouts.

Students will be able to:

-   use RJAGS package in R, by using the reference material, for the
    statistical analysis of Bayesian hierarchical models.

-   compute MC approximations of the posterior quantities of a given
    Hierarchical model

------------------------------------------------------------------------

Preview:
========

-   [Monte Carlo approximation: An intoduction for practical use in
    R](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/MCapproximators.nb.html)

-   Case study: Space shuttle Challenger disaster

    -   [Bernoulli model with conjugate priors
        (questions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/BernoulliModel_practical.nb.html)

    -   [Bernoulli model with conjugate priors
        (solutions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/BernoulliModel_full.nb.html)

    -   [Bernoulli regression model
        (questions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/BernoulliRegressionModel_practical.nb.html)

    -   [Bernoulli regression model
        (solutions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/BernoulliRegressionModel_full.nb.html)

    -   [Bernoulli regression model -variable selection
        (questions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/BernoulliRegressionModelVS_practical.nb.html)

    -   [Bernoulli regression model -variable selection
        (solutions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/BernoulliRegressionModelVS_full.nb.html)

    -   [Normal Mixture model
        (solutions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/BayesianNormalMixtureModel.nb.html)

-   Exercises for practise :

    -   [Normal model
        (questions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/NormalModel_practical.nb.html)

    -   [Normal model
        (solutions)](http://htmlpreview.github.io/?https://github.com/georgios-stats/Bayesian_Statistics/blob/master/ComputerPracticals/output/NormalModel_full.nb.html)

------------------------------------------------------------------------

Reference list
==============

*The material below is not examinable material, but it contains
references that students can follow if they want to further explore the
concepts introdced.*

-   References for *RJAGS*:
    -   [JAGS homepage](http://mcmc-jags.sourceforge.net)  
    -   [JAGS R CRAN
        Repository](https://cran.r-project.org/web/packages/rjags/index.html)  
    -   [JAGS Reference
        Manual](https://cran.r-project.org/web/packages/rjags/rjags.pdf)  
    -   [JAGS user
        manual](https://sourceforge.net/projects/mcmc-jags/files/Manuals/4.x/jags_user_manual.pdf/download)
-   Reference for *R*:
    -   [Cheat sheet with basic commands for
        *R*](https://www.rstudio.com/wp-content/uploads/2016/10/r-cheat-sheet-3.pdf)
-   Reference of *rmarkdown* (optional)
    -   [R Markdown
        cheatsheet](https://www.rstudio.com/wp-content/uploads/2016/03/rmarkdown-cheatsheet-2.0.pdf)  
    -   [R Markdown Reference
        Guide](http://442r58kc8ke1y38f62ssb208-wpengine.netdna-ssl.com/wp-content/uploads/2015/03/rmarkdown-reference.pdf)  
    -   [knitr options](https://yihui.name/knitr/options)
-   Reference for *Latex* (optional):
    -   [Latex Cheat
        Sheet](https://wch.github.io/latexsheet/latexsheet-a4.pdf)

------------------------------------------------------------------------

Setting up the computing environment
====================================

### CIS computers

From AppHub, load the modules:

1.  Google Chrome

2.  LaTex

3.  rstudio

### Your personal computers (Do not do it on CIS computers)

There is not need to do this in CIS computers as the required foftware
is (supposed to be) properly installed.

The instructions below are at your own risk…

We recommend the use of LINUX operation system.

Briefly, you need to do the following:

1.  Install LaTex (optional but recommended)
    -   Source: download it from
        <https://www.tug.org/texlive/acquire-netinstall.html>
    -   Debian: *apt-get install texlive-full*  
    -   Fedora: *yum install texlive texlive-latex*  
    -   windows: download it from
        <https://miktex.org/howto/install-miktex>
    -   macos: download it from <https://www.tug.org/mactex/>
2.  Install R computing environment version R 2.14.0 or later.
    -   Source: download it from here: <https://cran.r-project.org/>  
    -   Debian: *sudo apt install r-base*  
    -   Fedora: *yum install -y R*  
    -   windows: download it from <https://cran.r-project.org/>
        -   I recomend tyou to install *Rtools* as well, for you to be
            able to instal R packages.  
    -   macos: download it from <https://www.tug.org/mactex/>
3.  Install the latest Rstudio (recommended)
    -   Any OS: Download it from here:
        <https://www.rstudio.com/products/rstudio/download/>

### Install of JAGS

For any OS:

Details for installing JAGS can be found in:

-   <http://mcmc-jags.sourceforge.net/>

-   <https://cran.r-project.org/web/packages/rjags/INSTALL>

Briefly:

1.  Uninstall any existing RJAGS if possible. In R terminal run:  
    `> remove.packages("rjags")`  
    `> if (file.exists(".RData")) file.remove(".RData")`

2.  Restart R

3.  Install RJAGS. In R terminal run:  
    `> install.packages("rjags", repos = "https://cloud.r-project.org/", dependencies = TRUE)`

### This handout

To download this handout, run rstudio, and do the following

1.  Go to File &gt; New Project &gt; Version Control &gt; Git

2.  In the section *Repository URL* write

-   <https://github.com/georgios-stats/Bayesian_Statistics.git>

-   … and complete the rest as you wish

1.  Hit *Create a Project*

…this will download some material of the course. This handout is in
folder *PracticalHandout*.

.
