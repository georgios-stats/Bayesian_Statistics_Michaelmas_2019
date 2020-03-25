------------------------------------------------------------------------

# Details

------------------------------------------------------------------------

### Description:

This repository contains the teaching material for the module MATH3341/4031 Bayesian statistics III/IV.

-   '[Description.pdf](https://github.com/georgios-stats/Bayesian_Statistics/blob/master/Description.pdf)' contains the ILOs, sylabus, and bibliography

### Lectures and Problem classes

-   '[LectureHandouts](https://github.com/georgios-stats/Bayesian_Statistics/tree/master/LectureHandouts#details-about-lecture-material)' folder contains the material used in your lectures and problem classes

### Computer practicals classes

-   '[ComputerPractical](https://github.com/georgios-stats/Bayesian_Statistics/tree/master/ComputerPracticals#details-about-computer-practicals)' folder contains the material for your computer practicals

### Homework

-   '[Homework](https://github.com/georgios-stats/Bayesian_Statistics/tree/master/Homework#details-about-exercise-material)' folder contains the material used for your practice at home

### Web-applets

-   '[Shiny_applets](https://github.com/georgios-stats/Bayesian_Statistics/tree/master/Shiny_applets#shiny-applets)' folder contains the source code of the web applets used in the lectures.


### Introductory videos

- ***Tony O'Hagan interviews Dennis Lindley about Bayesian Stats @RSS:***  
***Topics:*** Bayesian stats foundations, subjectivism, inference; How it Bayesain stats were developed.

     [<img src="https://img.youtube.com/vi/cgclGi8yEu4/0.jpg" alt="drawing" width="100"/>](https://www.youtube.com/watch?v=cgclGi8yEu4)

- ***Jim Berger is interviewed about Bayesian inference @Duke University:***  
***Topics:*** Bayesian inference, its uncertainty quantification applications, comparisons against Frequentists.

     [<img src="https://img.youtube.com/vi/3eZ5yg6g_Fc/0.jpg" alt="drawing" width="100"/>](https://www.youtube.com/watch?v=3eZ5yg6g_Fc)

------------------------------------------------------------------------

# How to download:


### To download the whole repository

Ways:

1. You can click [[HERE](https://github.com/georgios-stats/Bayesian_Statistics/archive/master.zip)].

2. You can click the green button 'Clone or download' and download it as a zip file

3. You can use the program 'git' (<https://git-scm.com/>):
    
    -   in windows/linux: 
    
        download and install git from https://git-scm.com/
    
    -   in Debian linux run in the terminal: 
    
        sudo apt-get install git
    
    -   in Red Hat linux run in the terminal: 
    
        sudo yum install git
    
    ... then run:

    -   git clone https://github.com/georgios-stats/Bayesian_Statistics.git

4. You can use rstudio:

    1.  Go to File &gt; New Project &gt; Version Control &gt; Git
    
    2.  In the section *Repository URL* write
        
        -   <https://github.com/georgios-stats/Bayesian_Statistics.git>
        
        -   … and complete the rest as you wish
    
    3.  Hit *Create a Project*

### To download a specific folder only

Ways:

1. You can use the GitZip add-on for Firefox available [HERE](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&cad=rja&uact=8&ved=2ahUKEwias52xjd3nAhXPUs0KHeXHCEUQFjACegQIAhAB&url=https%3A%2F%2Faddons.mozilla.org%2Fen-US%2Ffirefox%2Faddon%2Fgitzip%2F&usg=AOvVaw37servrJ29tuNcx9dIQDqy) or the Chrome add-on GitZip available [HERE](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=2ahUKEwias52xjd3nAhXPUs0KHeXHCEUQFjABegQIARAB&url=https%3A%2F%2Fchrome.google.com%2Fwebstore%2Fdetail%2Fgitzip-for-github%2Fffabmkklhbepgcgfonabamgnfafbdlkn%3Fhl%3Den&usg=AOvVaw1Pn3VXuXz1Fphl7dsPEhDS)

    1. In install [Firefox GitZip add-on](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&cad=rja&uact=8&ved=2ahUKEwias52xjd3nAhXPUs0KHeXHCEUQFjACegQIAhAB&url=https%3A%2F%2Faddons.mozilla.org%2Fen-US%2Ffirefox%2Faddon%2Fgitzip%2F&usg=AOvVaw37servrJ29tuNcx9dIQDqy) or the [Chrome GitZip add-on](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=2ahUKEwias52xjd3nAhXPUs0KHeXHCEUQFjABegQIARAB&url=https%3A%2F%2Fchrome.google.com%2Fwebstore%2Fdetail%2Fgitzip-for-github%2Fffabmkklhbepgcgfonabamgnfafbdlkn%3Fhl%3Den&usg=AOvVaw1Pn3VXuXz1Fphl7dsPEhDS)  

    2. Double click on the items you need.  
    
    3. Click download button at bottom-right.  
    
    4. See the progress dashboard and wait for browser trigger download.  
    
    5. Get the ZIP file.  

2. You can use 'git' (<https://git-scm.com/>). 

    E.g., assume you wish to download the sub-folder 'ComputerPractical':

    -   run in the terminal the following:
        
        *mkdir Bayesian_Statistics  
        cd Bayesian_Statistics  
        git init  
        git remote add -f origin https://github.com/georgios-stats/Bayesian_Statistics.git  
        git config core.sparseCheckout true  
        echo "ComputerPracticals/*" >> .git/info/sparse-checkout  
        git pull origin master*

### To download a specific file

1. You can just navigate to the file from the browser and download it.

2. You can use the GitZip add-on for Firefox available [HERE](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&cad=rja&uact=8&ved=2ahUKEwias52xjd3nAhXPUs0KHeXHCEUQFjACegQIAhAB&url=https%3A%2F%2Faddons.mozilla.org%2Fen-US%2Ffirefox%2Faddon%2Fgitzip%2F&usg=AOvVaw37servrJ29tuNcx9dIQDqy) or the Chrome add-on GitZip available [HERE](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=2ahUKEwias52xjd3nAhXPUs0KHeXHCEUQFjABegQIARAB&url=https%3A%2F%2Fchrome.google.com%2Fwebstore%2Fdetail%2Fgitzip-for-github%2Fffabmkklhbepgcgfonabamgnfafbdlkn%3Fhl%3Den&usg=AOvVaw1Pn3VXuXz1Fphl7dsPEhDS)


------------------------------------------------------------------------

