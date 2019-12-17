

------------------------------------------------------------------------

About:
======

This repository contains the teaching material for the module MATH3341/4031 Bayesian statistics III/IV.

It contains 4 main folders: 

-   'ComputerPractical' which contains the material for your computer practicals

-   'Homework' which contains the material used for your practice at home

-   'LectureHandouts' which contains the material used in your lectures and problem classes

-   'Shiny_applets' which contains the source code of the web applets used in the lectures.

------------------------------------------------------------------------

How to download:
===============

As a pre-requisite, to use the command 'git' you need to download and install the software git from 'https://git-scm.com/':

-   in windows/linux: 

    download and install git from https://git-scm.com/

-   in Debian linux run in the terminal: 

    sudo apt-get install git

-   in Red Hat linux run in the terminal: 

    sudo yum install git

To download all the repository you can run:

-   git clone https://github.com/georgios-stats/Bayesian_Statistics.git

or

-   click the green button 'Clone or download' and download it as a zip file

To download a specific folder only, e.g. the 'ComputerPractical', you can run in the terminal the following:

        mkdir Bayesian_Statistics
        cd Bayesian_Statistics
        git init
        git remote add -f origin git remote add -f origin
        git remote add -f origin https://github.com/georgios-stats/Bayesian_Statistics.git
        git config core.sparseCheckout true
        echo "./ComputerPracticals" >> .git/info/sparse-checkout
        git pull origin master

To download a specific file, you can just navigate to the file from the browser and download it.

------------------------------------------------------------------------

