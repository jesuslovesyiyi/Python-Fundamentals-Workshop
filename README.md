# Python-Fundamentals-Workshop

## Workshop Goals

This interactive workshop is your complete introduction to programming Python for people with little or no previous programming experience, with a focus on data science applications. It covers the basics of Python and Jupyter, variables and data types, and a gentle introduction to data analysis in Pandas.

The materials of this workshop were first developed by the Berkeley Dlab. I made modifications to the original code to suit the purpose of this course.
## Learning Objectives

After completing Python Fundamentals, you will be able to:
- Navigate Jupyter Notebooks.
- Assign variables.
- Distinguish common data types and structures.
- Apply methods to data types.
- Perform basic operations in Pandas.
- Inspect documentation to deal with error messages.

## Workshop Structure

1. **Part 1: Introduction to Jupyter and Python**
2. **Part 2: Data Types and Structures**
3. **Part 3: Introduction to Pandas**

## Installation Instructions
**Option A: Install Anaconda**

Anaconda is software that allows you to run Python and Jupyter notebooks on your computer. Installing Anaconda is the easiest way to make sure you have all the necessary software to run the materials for this workshop.

<u>Preliminaries</u>

1. Read the Anaconda QuickStart guide (https://docs.continuum.io/anaconda/install).

2. Read the Jupyter Notebook overview: (http://jupyter-notebook.readthedocs.io/en/latest/notebook.html).

3. If you are not already comfortable with the command prompt (windows) or terminal (Mac), please read (http://dosprompt.info/). to familiarize yourself with the basic commands (such as changing directories and listing the contents of a directory) discussed in these links so that you can use the command prompt/terminal to access Python.

<u>Download and install Anaconda</u>

1. [Download and install Anaconda (Python 3.12 distribution)](https://www.anaconda.com/products/individual). Click "Download" and then click 64-bit "Graphical Installer" for your current operating system.
2. Make sure you download the correct installer for your operating system (Windows, Mac, Linux, etc) and architecture (32 or 64-bit). If you don't know if your operating system is 32 or 64-bit, Google will show you how to check it.  And make sure you download the installer for Python 3.12, not 2.7.
3. Run the Anaconda installer.
4. In the Anaconda installer dialog, choose to install for all users, set the destination folder to c:\anaconda (or the equivalent if you're on a Mac), and make sure both tick boxes are ticked for "add anaconda to the system path" and "register anaconda as the system python"

**Option B: Install Miniconda**

Miniconda is a minimal version of the Anaconda Python distribution, which includes only the necessary components required to run Python and manage packages. It provides a lightweight, command-line tool that simplifies the installation and management of software dependencies, making it an excellent choice for developers who prefer a more streamlined approach.

1. Visit the Miniconda website (https://docs.conda.io/en/latest/miniconda.htmlLinks to an external site.).
2. Choose the appropriate installer for your operating system (Windows, macOS, or Linux).
3. Download the installer and run it.
4. Follow the on-screen instructions to complete the installation.

Once the installation is complete, you can open a terminal or command prompt to verify that Miniconda has been installed correctly by running the following command:
```
conda --version
```
If the command displays the version of Conda, you have successfully installed Miniconda.

## Download the materials in this repository:

* Click the green "**Code**" button in the top right of the repository information.
* Click "**Download Zip**".
* Extract this file to a folder on your computer where you can easily access it (I recommend Desktop).

Optional: if you're familiar with `git`, you can instead clone this repository by opening a terminal and entering
```
git clone https://github.com/jesuslovesyiyi/Python-Fundamentals-Workshop.git
```

## Run the code

Now that you have all the required software and materials, you need to run the code. Below are steps you will take to run the code using Anaconda.

1. Open the Anaconda Navigator application. You should see the green snake logo appear on your screen. Note that this can take a few minutes to load up the first time.

2. Click the "Launch" button under "Jupyter Lab" and navigate through your file system to the `Python-Fundamentals-Workshop` folder you downloaded above.

3. Navigate to "**lessons**"

4. Open the `01_Jupyter_and_Python.ipynb` to begin.

5. Press `Shift + Enter` (or `Ctrl + Enter`) to run a cell.


## Virtual Environments
To create a new virtual environment, follow these steps:

1. Open a terminal or command prompt.
2. Run the following command to create a new virtual environment:
```
conda create --name myenv python=3.12
```
Replace `myenv` with the desired name for your virtual environment. Conda will create a new environment with the specified name and install a minimal set of packages.

Once you have created a virtual environment, you need to activate it to start using it. Follow these steps:

1. Open a terminal or command prompt.
2. Activate the environment using the following command:

For Windows:
```
conda activate myenv
```

For macOS and Linux:
```
source activate myenv
```

The name `myenv` should match the name of the environment you created in the previous step.

To deactivate the virtual environment and return to the global Python environment, use the following command:

For Windows:
```
conda deactivate
```

For macOS and Linux:
```
source deactivate
```

With the virtual environment activated, you can now install Python packages specific to your project. Use the conda install or pip install command to install packages, just like you would in a regular Python environment. For example:
```
conda install numpy
```
```
pip install pandas
```
To ensure stability and avoid conflicts between math libraries (like MKL and OpenBLAS), it's best to install core scientific packages using a single package manager. We recommend using Conda for packages like NumPy, Pandas, SciPy, and Matplotlib.

For this workshop, **install the necessary packages** by running the following command:

```
conda install numpy pandas matplotlib
```

To add a virtual environment to Jupyter Notebook you will need to first install ipykernel which provides the IPython kernel for Jupyter:

```
pip install ipykernel
```
Next you can add your virtual environment to Jupyter by typing:
```
python -m ipykernel install --user --name=myenv
```
Again, the name `myenv` should match the name of the environment you created before.

## VS Code
Visual Studio Code (VS Code) is a popular code editor that provides excellent support for Python development. To download and install VS Code: https://code.visualstudio.com/download.

To get started with VS Code please check out their official website: https://code.visualstudio.com/docs/getstarted/getting-started.

To integrate Anaconda and Miniconda with VS Code, follow these steps:
1. Install the “Python” extension within VS Code.

- Go to the **Extensions** view by clicking on the Extensions icon in the Activity Bar on the side of the window or by pressing `Ctrl+Shift+X`.

- In the search bar, type `Python`.

- Select the extension published by Microsoft and click Install.

2. Select the Conda environment.

- Open your project folder in VS Code.

- Open the Command Palette by pressing `Ctrl+Shift+P`.

- Type `Python: Select Interpreter` and press Enter.

- A list of available Python interpreters will be displayed, including those from your Conda environments. Select the Conda environment you wish to use (e.g., `'my-env': conda`).

You have now successfully configured VS Code to use your Conda environment.

For other settings, please refer to https://code.visualstudio.com/docs/languages/python#_configuration



# Python-Fundamentals-Workshop in Colab

## Download the materials in this repository:

* Click the green "**Code**" button in the top right of the repository information.
* Click "**Download Zip**".
* Extract this file to a **folder** on your computer where you can easily access it.

## Upload the folder into Google Drive

- Upload the **folder** into your **Google Drive** (persistent, recommended).
- In your Google Drive, create a folder named `repos`.
- Place the entire repository folder inside it, so that the path looks like:

![](/img/MyDrive_repos.png)

- The folder structure in your Drive should match the example shown in the figure. Please make sure your Drive looks the same as the screenshot, otherwise Colab may not find the files correctly.

## Locate the repository in Colab

- In Google Drive, double-click to open the **Python-Fundamentals-Workshop** folder, then open the **lessons** folder, and finally open **1_Jupyter_and_Python.ipynb**.

- At the top of the notebook, run the following code (Colab may ask you to grant Drive access—click **Connect to Google Drive** and continue):

```
from google.colab import drive
drive.mount('/content/drive')
%cd /content/drive/MyDrive/repos/Python-Fundamentals-Workshop/lessons
!ls
```

- You can now run all the code in Colab (the Colab environment already includes all the packages required for this workshop).
- The figure below shows the expected output once the setup is successful:

![](/img/drive_mount.png)

- For the other two `.ipynb` files, follow the same steps—you also need to run the code at the top of the notebook to ensure access to the required datasets in the repository.