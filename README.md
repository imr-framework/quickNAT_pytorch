<h1 align="center"> quickNAT pytorch tutorial </h1> <br>

PyTorch implementation of QuickNAT is a fast brain MRI segmentation framework [1]. This tutorial is created to help students in BMEN 6003 Computational Modeling of Physiological Systems class to set up and use this package. If you have any questions, please contact the author of this tutorial. The tutorial is written based on Windows system, but MacOS should be similar. 

## Python Installation
1. Please go to [Python](https://www.python.org/) to download Python based on your OS. The recommended version is **Python 3.6.3** as it is the version that we are currently running QuickNAT on. 

2. Run the installer after downloading is completed. Please check the box **add Python to PATH**. This adds your Python path to your system path. 

3. After installation is completed, we can check if Python is installed succesfully using `python --version` command in command prompt. It should display the Python version installed. 

## Pip Installation
pip is a standard package install/management system written in Python. We will be using it to install and manage our packages. 

1. Now that we have Python, we can check if pip is available. Type `pip --version` in command prompt to check your pip version. If the command is not recognized, it means pip is not available and we need to manually install it. If it is available, you can skip this section.

2. Go to [pip](https://pip.pypa.io/en/stable/installing/) and download **get-pip.py** to your Python path. You can check your Python path using `python -c "import sys; print(sys.executable)"`.

3. Direct your command prompt to your Python path. You can do it by `cd YourPythonPath`.

4. Use `python get-pip.py` to install pip. After the installation is completed, we can check pip version using `pip --version`

5. Make sure pip is up to date, if not, please update your pip to latest version. You can do that by `python -m pip install -U pip`

## Jupyter notebook installation
1. Use `python -m pip install jupyter` to install Jupyter notebook.

2. We can start Jupyter notebook using `jupyter notebook`

## Virtual environment installation
Virtual environment is extremly useful when working with many different projects. Each virtual environment is independent of each other and we can install packages needed for each specific project. 

1. Direct your command prompt to the location where you want to keep your virtual environments.

2. Use `python -m venv myenv` to create a virtual environment at specified location. You can change `myenv` to any name you prefer. We can check if the virtual environment is succesfully created by checking if the folder exist in specified location. 

3. Update pip if needed using method described above. 

4. Run **activate** under the **Scripts** folder in your virtual environment to activate your virtual environment. We can check what packages are already installed using `pip list`.

5. After virtual environment is activated, we can install software packages needed for this project.

5. To exit from virtual environment, we can run **deactivate** under the **Scripts** folder in the virtual environment folder.

## Connect virtual environment to Jypyter notebook
1. First activate your virtual environment using method described above. 

2. Install IPython kernel to Jupyter notebook using `pip install --user ipykernel`

3. Add your virtual environment to Jupyter notebook using `python -m ipykernel install --user --name=myenv`

4. Open Jupyter notebook, you should be able to select your virtual environment now. 
