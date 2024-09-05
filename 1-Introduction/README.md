## Run Jupyter Notebooks

### 1. Run in GBLearn
You can run the Jupyter notebooks in GBLearn. To do this, follow this [instruction](./gblearn%20python%20jupyter%20notebook%20setup.pdf).


### 2. Run locally on your machine

**Step 1:** Insatall VS Code and Python extension

**Step 2:** Check if Python is installed. To check this run the following command in the terminal.
```bash
python --version
```
or
```bash
python3 --version
```

**Note:** For Mac users python will be installed after adding python extension to VS Code. For Windows users, if python is not installed, download and install it from Microsoft Store.


**Step 3:** Create a virtual environt through the terminal:

```bash
python -m venv .venv
```

and then activate the vrirtual environment in the terminal by running the following command:

```bash
.venv\Scripts\activate
```

or (for Mac users)

```bash
source .venv/bin/activate
```


**Note:** For Windows users this command may raise an error. In this case change your terminal from `PowerShell` to `Command Prompt`. You can do it in VS Code by going to the terminal and clicking on the dropdown menu and selecting `Command Prompt`.

**Step 4:** Open the Jupyter notebook in VS Code. When you open the notebook for the first time in VS Code, it will ask you to install the Jupyter extension. Click on the install button to install the Jupyter extension.

**Step 5:** Go to the right top side of the Jupyter Notebook in 
VS Code and select the kernel as the virtual environment you created.

**Note:** If your virtual environment isn't showing up, you can manually add it to Jupyter with the following command:

```bash
python -m ipykernel install --user --name=myenv
```
Replace myenv with the name of your virtual environment. This command registers the virtual environment as a Jupyter kernel.


**Additional Notes:** 

Watch this [video](https://drive.google.com/file/d/1la5G4q_cjCHWU4myUb5CH_rpaXdbKCG7/view?usp=sharing) to create a jupyter notebook in VS Code and run it locally in a virtual environment.

A detailed guide on how to create a virtual environment without VSCode is in [setup_instruction.md](setup_instruction.md)


## Cloning the course repository on your local machine

Clone the repository in the directory. 
```bash
git clone https://github.com/kamrik/PyData2024.git
```

Then navigae to the cloned repository and open the notebooks is VS Code. 
```bash
cd PyData2024
```

**Note:** Read the details about repo cloning in this [Link](../0-GitHub_Lessons/lesson_1.md).


