# Python Basics Tutorial

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Run Conda commands to create a new Conda environment for this assignment.
- [ ] Open the repository Jupyter Notebook in VSCode or Jupyter Notebooks.
- [ ] Add the code shown in this video to your Jupyter Notebook.
- [ ] Push your updated file to your GitHub repository.
- [ ] Answer assignment questions and submit a link to this GitHub repository in Canvas.
- [ ] Remove your virtual environment from Jupyter Notebooks and from your machine.

## Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/N6806_Fall2020_DevNotes/blob/master/Projects/002%20-%20Practice%20Using%20Git%20and%20GitHub/README.md
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.

## Create a new Conda environment for this assignment.

* This can be done directly in VSCode
  * Open a new terminal in VSCode.
  * If you know the packages you will use for the project, you can install the packages at the same time you create the new environment using Conda. For this assignment we will install ipykernel so we can add the new environment to Jupyter Notebook.
  * In the terminal window run the command `conda -V` to check Conda is installed and is in your path.
  * To see a list of available Python versions run the command `conda search "^python$"`
  * To simply create an environment using the same version of Python already installed on your machine with the packages you want run the command `conda create --name myenv` with the packages you want listed after the environment name.
  * For this assignment I'll create an environment named Basics with package ipykernel (allows us to use the new environment with Jupyter Notebook) with command `conda create --name Basics ipykernel`
  * This will take a few minutes while the packages and dependencies are installed in the new environment.
  * Verify your new environment exists by running command `conda env list`
  * We'll be doing this assignment in a Jupyter Notebook in Anaconda or VSCode. Activate your new environment by running the command `source activate Basics`. Add the kernel for your new environment to Jupyter Notebook by running the command `python -m ipykernel install --user --name=Basics`.
  
## Open the repository Jupyter Notebook
* Open Jupyter Notebook on your machine.
* In the Files tab you should see folders that match the folders on your machine (i.e. Desktop, Documents, Downloads). Navigate to your repository folder by clicking on the folder links. Open the .ipynb file in your repository by clicking on it.
* When your repository workbook opens in your browser window, make sure you're using your assignment workbook with the new environment by going to Kernel - change kernel - select dataVis


## Follow along with this tutorial

* Complete the Learn the Basics section at: https://www.learnpython.org/
  * Enter each code section in a separate cell and run it in your Jupyter Notebook file.
  * An easy short cut is to hit Shift-Enter after you've entered the code in a cell. This runs the cell and creates a new one below for the next code block.
  * When you're done make sure you save your file.

## Push your updated file to your GitHub repository

* This can be done in VSCode.
  * In VSCode click on the Source Control button.
  * You should see the files that had changes. (Mine has the original file which shows an M next to it and a new file which says checkpoint in the name. You really only need to push the original file, but if you push both it shouldn't hurt anything.)
  * Hover over the changed file. Click the + sign to stage the change.
  * Enter a commit message in the message field and click the checkmark to commit the change.
  * Click on the 3 dots for more actions and select Sync. This will push the updated file to your GitHub repository.
  * Submit the link to your GitHub repository on Canvas.
  
## Remove your virtual environment

* You can remove your virtual environment for this assignment from your Jupyter Notebook and your computer.
* In the terminal run the code `jupyter kernelspec list` to see what environments are available for your notebooks.
* To remove the environment from your Jupyter Notebooks run the code `jupyter kernelspec uninstall Basics`.
* Get a list of the environments in Conda run `conda env list`.
* To delete an environment and everything in it run `conda env remove --name Basics`.
