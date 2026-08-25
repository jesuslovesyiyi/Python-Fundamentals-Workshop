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



Before starting the workshop, please set up **Anaconda**, **VS Code**, and a Conda environment for running Jupyter Notebooks.

> **Please carefully read the official documentation linked below.** Most of the information you need for installation, environment setup, and troubleshooting is already provided there. The steps here are only a short guide to the setup we will use in this workshop.

## Installation Instructions

### 1. Install Anaconda

Download and install **Anaconda Distribution** for your operating system:

https://www.anaconda.com/docs/getting-started/installation

After installation, open **Anaconda Prompt** on Windows or **Terminal** on macOS/Linux and check that Conda works:

```
conda --version
```

### 2. Create a Conda environment and install the required packages

Create a Conda environment for the workshop and install the required packages:

```
conda create -n python-fundamentals python=3.12 jupyter ipykernel numpy pandas matplotlib
```

When prompted, type `y` and press **Enter** to continue.

Activate the environment:

```
conda activate python-fundamentals
```

We use `python-fundamentals` as the environment name in this guide, but you may choose a different name. If you do, replace `python-fundamentals` with your chosen environment name in the commands below.

For more information about creating, activating, and managing Conda environments, please review:

https://www.anaconda.com/docs/getting-started/working-with-conda/environments

Finally, register the Conda environment as a Jupyter kernel:

```
python -m ipykernel install --user --name=python-fundamentals --display-name "Python (python-fundamentals)"
```

This allows you to select the environment when running Jupyter Notebooks. If you chose a different environment name, update both `--name` and `--display-name` accordingly.

### 3. Download the materials

First, download the workshop materials from this repository.

1. Click the green **Code** button near the top of the repository.
2. Click **Download ZIP**.
3. Extract the ZIP file to a folder on your computer that you can easily access.

If you are familiar with Git, you may instead clone the repository:

```
git clone https://github.com/jesuslovesyiyi/Python-Fundamentals-Workshop.git
```

### 4. Open the notebooks

There are **two options** for opening the workshop notebooks. You only need to use one.

#### Option 1: Use Jupyter Notebook through Anaconda

You can run the workshop notebooks using **Jupyter Notebook**.

1. Open **Anaconda Navigator**.
2. Find **Jupyter Notebook** and click **Launch**.
3. A browser window will open showing your files and folders.
4. Navigate to the `Python-Fundamentals-Workshop` folder you downloaded.
5. Open the `lessons` folder.
6. Open `01_Jupyter_and_Python.ipynb`.
7. Make sure the notebook is using the kernel you created, such as **Python (python-fundamentals)**.
8. Press `Shift + Enter` to run a cell.

You can also start Jupyter Notebook from **Anaconda Prompt** or **Terminal**:

```
conda activate python-fundamentals
jupyter notebook
```

#### Option 2: Use VS Code

**Visual Studio Code (VS Code)** is a popular code editor with excellent support for Python and Jupyter Notebooks.

To download and install VS Code, please follow the official instructions:

https://code.visualstudio.com/download

To use the Conda environment you created earlier in VS Code, please review:

https://code.visualstudio.com/docs/python/environments

We recommend spending some time setting up and becoming familiar with VS Code, as it is widely used for Python programming and will be beneficial for your future coursework and research project.

### 5. Check your setup

You are ready for the workshop if all of the following work:

1. In Anaconda Prompt or Terminal, activate your environment:

```
conda activate python-fundamentals
```

2. Confirm that Python is available:

```
python --version
```

3. Open `lessons/01_Jupyter_and_Python.ipynb` in Jupyter Notebook or VS Code.

4. Make sure the notebook is using your workshop environment as the kernel, such as **Python (python-fundamentals)**.

5. Add a new code cell and run the following code:

```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

print("Setup complete!")
```

If the cell runs without errors and prints:

```
Setup complete!
```

then your environment, required packages, and Jupyter kernel are set up correctly.