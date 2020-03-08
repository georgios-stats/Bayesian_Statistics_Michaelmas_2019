
# Shiny applets

Here is a list of interactive shiny applications related that can be used to understand as a suplamentary material. 

## How to run the Web Applets from the server 

You can click on the following links:  


+ For the demo presenting standard distributions  
  * <https://georgios-stats.shinyapps.io/demo_distributions/>    
      
+ For the demo presenting Multivariate distributions
  * <https://georgios-stats-3.shinyapps.io/demo_MultivariateNormalDistribution/> 
      
+ For the demo presenting Central Limit Theorem  

  * <https://georgios-stats.shinyapps.io/demo_clt/>  
      
+ For the demo presenting the Weak Law of Large Numbers  

  * <https://georgios-stats.shinyapps.io/demo_wlln/>  
      
+ For the demo presenting the conjugate priors  

  * <https://georgios-stats-1.shinyapps.io/demo_conjugatepriors/>  
      
+ For the demo comparing Conjugate Jeffreys and Laplace priors  

  * <https://georgios-stats-1.shinyapps.io/demo_conjugatejeffreyslaplacepriors/>  
      
+ For the demo presenting the Mixture priors  

  * <https://georgios-stats-1.shinyapps.io/demo_mixturepriors/>  
      
+ For the demo presenting standard parametric/predictive Bayes point estimators  

  * <https://georgios-stats-1.shinyapps.io/demo_PointEstimation/>   
      
+ For the demo presenting Credible intervals   

  * <https://georgios-stats-1.shinyapps.io/demo_CredibleSets/> 

These applications are currently uploaded on non-Durham Univertity server, which means that we have only 25 active hours per mounth. If we exceed this limit, you will be able to run these applications localy on your computer by dowlnoaded them. (see below.)


## How to download the Web Applets and run them localy


In order to download, edit, run the Web Applets to your computer, do the following:

1. Run rstudio
  1. In the console run  
      * install.packages("rmarkdown")
  2. Go to File>New Project>Version Control>Git  
  3. In the section "Repository URL" type: 
      * https://github.com/georgios-stats/Shiny_applets.git    
  4. Then you can run the applications either by clicking and running each 'name'.Rmd script in the demo_'name', or by running the commands: 
      * For the demo presenting standard univariate distributions
          * rmarkdown::run("./demo_distributions/demo_distributions.Rmd")
      * For the demo presenting standard multivariate distributions
          * rmarkdown::run("./demo_MultivariateNormalDistribution/demo_MultivariateNormalDistribution.Rmd")
      * For the demo presenting Central Limit Theorem
          * rmarkdown::run("./demo_CLT/demo_CLT.Rmd")
      * For the demo presenting the Weak Law of Large Numbers
          * rmarkdown::run("./demo_WLLN/demo_WLLN.Rmd")
      * For the demo presenting the conjugate priors
          * rmarkdown::run("./demo_ConjugatePriors/demo_ConjugatePriors.Rmd")
      * For the demo comparing Conjugate Jeffreys and Laplace priors
          * rmarkdown::run("./demo_ConjugateJeffreysLaplacePriors/demo_ConjugateJeffreysLaplacePriors.Rmd")
      * For the demo presenting the Mixture priors
          * rmarkdown::run("./demo_MixturePriors/demo_MixturePriors.Rmd")
      * For the demo presenting standard parametric/predictive Bayes point estimators
          * rmarkdown::run("./demo_PointEstimation/demo_PointEstimation.Rmd")
      * For the demo presenting Credible intervals  
          * rmarkdown::run("./demo_CredibleSets/demo_CredibleSets.Rmd")
          
          
