# Setup instructions

If you wish to work locally, you should use a virtual environment. You can install one via Python’s native venv module (recommended) or via Anaconda. 

To uderstand why virtual environment is important whatch this [video](https://calmcode.io/course/virtualenv/intro).

## Python virtual environment

The first step is to install Python on your system. We recommend following [this](https://realpython.com/installing-python/) guide to get started.

When running a Python command in your terminal, such as python --version, you should think of the program running your command as the “main” Python on your system. We recommend keeping this main installation free of any packages, and using it to create separate environments for each application you work on — this way, each application can have its own dependencies and packages, and you won’t need to worry about potential compatibility issues with other applications.

In Python this is done with virtual environments, which are self-contained directory trees that each contain a Python installation with a particular Python version alongside all the packages the application needs. Creating such a virtual environment can be done with a number of different tools, but we’ll use the official Python package for that purpose, which is called venv. You can also use Anaconda to create virtual environments, but we’ll cover that in the next section.


```bash
# this will create a virtual environment
# called .comp3122 in your working directory
python -m venv ./.comp3122

# the first . is the current directory
```
Note: I use . before virtual environment names to remember that they are related to virtual envs. This is optional, but it’s a good practice to make names easily recognizable.

To activate and enter the environment, run `source ./.comp3122/bin/activate` on mac or `.\.comp3122\Scripts\activate`on windows in your working directory. To deactivate the environment, either run `deactivate` or exit the terminal. Note that every time you want to work on the labs, you should rerun activations commands mentioned above.

## Anaconda virtual environment

Anaconda is a popular distribution of Python that comes with a lot of pre-installed packages. It also comes with a package manager called conda, which can be used to create virtual environments. If you don’t have Anaconda installed, you can download it from [here](https://www.anaconda.com/products/distribution).

Once you have Anaconda installed, it makes sense to create a virtual environment for the course. 
To set up a virtual environment called `.comp3122`, run the following in your terminal:

```bash
# this will create an anaconda environment
# called .comp3122 in 'path/to/anaconda3/envs/'
conda create -n .comp3122 python=3.11

# 3.11 is the most up-to-date and secure version of python at the time of writing this guide.
```

To activate and enter the environment, run `conda activate .comp3122`. To deactivate the environment, either run `conda deactivate .comp3122` or exit the terminal. Note that every time you want to work on the labs or assignmen, you should rerun `conda activate .comp3122`.

Note: If you’ve chosen to go the Anaconda route, you can safely skip the next section and move straight to (section)Installing Packages.

## Installing packages
Once you’ve setup and activated your virtual environment (via conda or venv), you should install the libraries needed to run the assignments using pip. To do this we need to use a package manager. For python, the most common package manager is pip and for Anaconda, it’s conda.

```bash
# again, ensure your virtual env (either conda or venv)
# has been activated before running the commands below
cd <working_directory>  # cd to the labs directory

# install labs dependencies.
# since the virtual env is activated,
# this pip is associated with the
# python binary of the environment
pip install numpy
```

if you're using Anaconda, you can also install numpy using conda:

```bash
# numpy using conda
conda install numpy
```