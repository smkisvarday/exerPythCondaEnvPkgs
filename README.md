# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/exerGitPractice
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.
  * (2021 update: I recommend managing environments as shown in the new Anaconda introduction video. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial) If you want to try creating the environments using the user interface for Anaconda Navigator instead of the command line shown in the Conda What and Why tutorial, that's fine. But watch the Conda What and Why tutorial to understand some of the differences between Conda environments and other types of virtual environments available in Python.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |different environments are used for different purposes/projects|
|What is the default package manager in Python?            |pip|
|How do you manage environments and packages in Anaconda?  |conda package manager and virtual environment manager|
|`conda list`       |shows all the default packages that were installed|
|`conda env list`       |shows all the installed environments|
|How do you keep your base environment unchanged?       |create different environments|
|What is the link to the Conda cheat sheet?      |file:///C:/Users/Kisvarday/Desktop/Informatics/Utah/ComputerScience/conda-cheatsheet.pdf |
|`conda create --name XXXX`       |creates a new environment named XXXX|
|`source activate XXXX`       |designates that we will work in the environment named XXXX|
|`conda install YYYY`       |Installs package YYYY|
|channels in Conda       |path or location where python looks for the package that you want to install|
|`conda install -c ZZZZ YYYY`       |tell condo to look in channel named ZZZZ for the package named YYYY|
|`conda config --show channels`       |shows the channels that we have so far|
|`conda config --add channels ZZZZ`       |adds the channel ZZZZ to our channel list|
|conda-forge.org       |conda-forge.org is a community led collection of packages|
|`source deactivate`       |deactivates the environment|
|`conda config --get channels`       |Shows the priorities or order that conda will look at channels|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
#(da35) PS C:\Users\Kisvarday> conda deactivate da35
(base) PS C:\Users\Kisvarday> conda env list
# conda environments:
#
base                  *  C:\ProgramData\Anaconda3
ai37                     C:\Users\Kisvarday\.conda\envs\ai37
da35                     C:\Users\Kisvarday\.conda\envs\da35


```
* What command would you use to remove the environments you created for this exercise from your computer? |conda remove --name ENVNAME --all|

```
# conda remove --name ENVNAME --all

```
## 2021 Update
Python, Anaconda, and many programming languages are constantly evolving. The video Conda What and Why provides a great explanation of why you may want to use virtual environments for your Python projects, and it provides a nice demonstration of how to work in the command line. However, environment management using Anaconda Navigator is more user friently than ever. I personally will be using Anaconda Navigator to manage environments and packages since it seems easier to see what is going on using the GUI. If you haven't done so already watch the introduction to Anaconda video and pay close attention to the section on using Anaconda Navigator to create environments and install packages. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial
