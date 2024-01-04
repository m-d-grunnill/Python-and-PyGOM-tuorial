# Python and PyGOM tutorial


## Abstract
Python is one of the most commonly used coding languages, hosting an extensive array of packages in Data Science, Mathematics and Machine Learning. With a syntax that emphasis readability, Python is considered one of the easiest coding languages to learn. It is also free and open source. Therefore, Python code produced in a research project can be more easily shared with others and is more accessible outside of academic institutions. In this class, we will begin by introducing Jupyter Notebook (the medium in which this practical will be given) and the basics of python. We will then introduce the package Numpy and Pandas. Numpy provides support for handling multidimensional arrays and matrices. Pandas provides access to Dataframe and Serries objects. Dataframes being similar to spreadsheets, with Serries being a one-dimensional variant. The final section of this class with introduce PyGOM. PyGOM provides a toolbox for modeling with Ordinary Differential Equations (ODEs). Having been developed by the UK Health Security Agency, PyGOM has an emphasis on epidemiological modelling. Providing functionality not only for solving ODEs, parameter estimation and stochastic simulation, but methods for deriving the basic reproduction number R<sub>0</sub>. 

## Instructions

The tutorial is given Jupyter Notebook "Python_and_PyGOM.ipnyb". Before using the notebook you will need to follow the installation instructions below.
To use the notebook open Anaconda prompt use the command:
* `conda activate pygom`
* `cd *directory housing ""*` to navigate to the diretory housing "Python_and_PyGOM.ipnyb"
* `jupyter notebook` This should open a web browser window. Double click "Python_and_PyGOM.ipnyb" to open it and begin tutorial.

## Installation Instructions

### 1. Installing Python and Desired packages

1. Go to [Anaconda's installation manual](https://docs.anaconda.com/free/anaconda/install/index.html) and follow instructions for installing anaconda for your particular OS.
2. Once installed navigate to your programs/apps to anaconda->Anaconda prompt. Open anaconda prompt, if in you are running windows you may need to right click and select More->Run as Administrator.
3. Within Anaconda prompt execute the commands:
   1. `conda create --name pygom python==3.11.7` select y when prompted.
   2.	`conda activate pygom`
   3.	`pip install notebook dask matplotlib enum34 pandas python-dateutil numpy scipy sympy seaborn tqdm`

### 2. Installing PyGOM

#### 2.1 Installing git.
PyGOM's setup.py installation file need git to check which version it is. To install git download the installation file 
from git's website below, open the installation file and follow instructions.
* [https://git-scm.com/download](https://git-scm.com/download)

#### 2.2 Installing Microsoft C++ Build Tools (Windows OS ONLY)
PyGOM and a few other python packages require a C++ compiler. Unfortunately, Windows does not come with one. If you do not have a Windows machine skip the next section and go to section 2.2.
1. Go to this link and download Microsoft C++ Build Tools: https://visualstudio.microsoft.com/visual-cpp-build-tools/.
2. Download Microsoft C++ Build Tools:

![image info](./readme_images/Download%20Microsoft%20C++%20Build%20Tools.png)
3. Once downloaded open vs_BuildTools.exe and navigate too “Available”:

![image info](./readme_images/Available.png)
4. Select installation of community edition:

![image info](./readme_images/community_edition.png)

5. Select “Desktop development with C++”:

![image info](./readme_images/Desktop_development.png)
6. Optional: To save on memory you can deselect everything but “MSVC v143 – VS 2022 C++ x64/x86 build tools (Latest)” and “Windows [your version of Windows] SDK”:

![image info](./readme_images/memory_save.png)
7. Then click install:

![image info](./readme_images/install_build_tools.png)

8. Once installed Visual Studio may start simply close it.
9. Restart your computer.

#### 2.3	Installing PyGOM
Unfortunately installing PyGOM via pip is not currently working. However, pygom can be downloaded and then installed locally.

##### 2.3.1 Downloading PyGOM from GitHub
* If you are familiar with Git use the url [https://github.com/ukhsa-collaboration/pygom](https://github.com/ukhsa-collaboration/pygom) to clone PyGOM to your \*desired location\*.
* If you are not familiar with Git:
  1. Go to [PyGOM's GitHub repository](https://github.com/ukhsa-collaboration/pygom).
  2. Select Code->Download ZIP.
  3. Right click on the pygom-master.zip in the Downloads folder and select Extract All.
  4. Select \*desired location\* to extract pygom to by either typing the \*desired location\* in the field or selecting the Browse menu.
![image info](./readme_images/extracting_pygom.png)
  5. Click Extract.

##### 2.3.2 Installing PyGOM into the conda pygom environment.
1. Open Anaconda prompt, if in you are running windows you may need to right click and select More->Run as Administrator.
2. Enter commands: 
   1. `conda activate pygom`.
   2. `cd *desired location*`.
   3. `python setup.py install`.
3. Check pygom has been installed by entering the command `conda list` and looking for it in the output list of installed packages.




