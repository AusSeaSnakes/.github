# Code setup

In this setup, we use *Anaconda* for managing Python environments and *VS Code (by Microsoft)* for interpreting code. *Black* python package is used to format the code, and *Code Spell Checker* assists programmers in VS code. 
This setup uses the command prompt (also called terminal) to run some commands for installation (e.g. *conda create —name datasci*).
Note: This code setup was put together in 2023 for Windows 10 users.

*Git* is also used here to version control and backing up the code. Github hosts a copy of the code in a repository online (Github account). Here we use github.com/AusSeaSnakes/.github as the homepage to this Sea Snakes group for sharing Python code. *Git* and *Github* are easily integrated into VS code with a pre-installed GitHub extension in VS code.

## Anaconda installation/setup
1. Download [Anaconda Distribution](https://www.anaconda.com/products/distribution). Anaconda comes with the latest version of Python (no need to install Python directly). Anaconda was designed for scientists in mind and comes with many of the common packages required for scientific programming (e.g. matplotlib for plotting results).
2. Install Anaconda for “Just Me”, not all users, and Add it to your path! - Adding to your path means that you can use it directly from the terminal. Installing for Just Me means you can easily change the virtual environments without Global permissions - great when working on an organisation PC (e.g., university laptop).
3. Your Anaconda folder should have been installed in your “C:\Users\*username*” directory.
4. Check Anaconda (conda) is working by opening a command prompt/terminal and typing “conda”. This should print a long result with something like “conda is a tool for managing and deploying applications, environments and packages.” near the top.

## Create a virtual environment with Anaconda
```python
# Command Prompt Code:
conda create --name datasci # Create an environment for data science
# May have to type "y" to proceed...
conda activate datasci # Activate the environment
# Install packages with conda and pip:
conda install numpy scipy pandas matplotlib seaborn scikit-learn plotly 
pip install black
# May have to type "y" to proceed, and may take 5-10 minutes
conda list -n datasci # Check packages were install correctly
exit # Close the terminal
```
Notes:

- Virtual environments can be pretty large - 100s of MB to GBs - so don’t create too many! Try to create a new virtual environment for each big project. For example, [CoastSat](https://github.com/kvos/CoastSat) requires its own environment because it has very specific dependencies. Similarly, xarray (useful for analysing netcdf data) is another Python package that is best used in its own specific environment.
- Some useful commands with Anaconda in the command prompt;
    - To get back to the base environment use: *conda activate* rather than *conda activate datasci*
    - *conda info —envs* shows all environments you have
    - *conda remove -n myenv* removes the environment "myenv"

## VS Code installation/setup
1. Download [VS code](https://code.visualstudio.com/download)
2. Install VS Code to similar place as Anaconda (e.g. “C:\Users\*username*” directory)
3. Open VS Code and choose theme (e.g. Dark).
4. Sync to other devices - good to sign in with GitHub account if you have one!
5. Add *Python* extension. Also, add *Code Spell Checker* extension here. 
6. Choose a Project folder (e.g. create a project folder in your OneDrive where you store all project data)
7. Use “Ctrl+Shift+P” and choose “Python: Select Interpreter” to select the Python datasci environment. This will ensure your project uses the data science virtual environment via Anaconda. This means you don’t have to actually open Anaconda Navigator.

## Black Python formatter
Black will automatically format your code to the standard python format (e.g. 2 blank lines after importing packages and modules, two spaces before comments etc.). This is super useful and ensures your code is formatted consistently between projects.

1. Black is normally installed already if you have followed the above process. If not, install using the command prompt/ terminal via:

```python
conda activate datasci
pip install black
```

2. Set up VS code to apply formatting when python scripts are saved:
    1. VS Code settings (bottom left)
    2. Find Text Editor > Formatting > Editor: Format On Save
    3. Select format on file
3. Test by saving a python script in VS Code. Saving the file formats the code.

## Git and Github

It is recommended that you first watch a video and read a little about Git and Github to understand the basics of Git and source control (version control).
- https://code.visualstudio.com/docs/sourcecontrol/overview
- https://code.visualstudio.com/docs/sourcecontrol/intro-to-git 

1. Create a GitHub account via github.com. Take note of your username and email.
2. Download Git (can be done via VS Code - Source Control on left side, or via an online search).
3. Install Git:
    1. Install Git to a similar place as Anaconda (e.g. “C:\Users\*username*” directory)
    2. Select Components: Default is okay.
    3. Default text editor: Can change to VS code here if this is your preference.
    4. Set default initial branch to “main” is recommended.
    5. Defaults otherwise.
4. Check installation: 

```python
# Check the git version with the command prompt or terminal:
git --version
```

5. Add username and email to the config data for *Git* via the command prompt*:*

```python
git config --global user.name "user_name" # Replace user_name with your username
git config --global user.email "email" # Replace email with your email
# For example, git config --global user.name "james-th94"
```

6. Open GitHub to create an initial repository:
    1. From your GitHub account online; Your Repositories > New.
    2. Give your repository a name, description, choose privacy and Add a README file and .gitignore file (choose Python), add a Licence (e.g., MIT) and Create!
    - e.g., Repository name: Test1, Description: Git with VS code for Python example. Privary: Private, Add a README file, etc.

7. Using *Git* in VS Code:
    1. Open VS Code and install the GitHub Pull Requests and Issues extension (from the left side panel).
    2. VS Code > Help > Welcome > Clone Git Repository.
    3. Search for your Git Repo that you just set up (e.g., Test1).
    4. Clone to a **Projects** folder where all your projects will sit (not inside a specific folder as this will create a New Specific Folder for this specific project).
    5. Open the new cloned repository in VS code
    6. Go to source control on the left side and “Pull” from the “…” menu, or search for >Git: Pull to ensure you have the latest data from your repository before making edits.

8. Test Git by editing the README.md file:
    1. Go to the Explorer in VS Code and open the README.md file
    2. Write something new (e.g. “This is my first git commit”).
    3. Go to Source Control (left side) and type “first change” in the message box to explain your first code change. This is where you explain any changes to the code.
    4. Commit change (and click Yes if a pop up occurs).
    5. Push the change to GitHub (similar to Git Pull, but now Git Push) with Sync Changes (Git Push).

9. Refresh GitHub online to check the change has reached your GitHub account

## Test your Python setup

1. With your Project/repository folder in VS code activated in the Explorer menu, create a new Python file (e.g. MyFirstPythonScript.py). Example below.

```python
# %% Import Packages
import numpy as np  # import numpy package
import matplotlib.pyplot as plt  # import pyplot module from matplotlib package
from datetime import datetime  # import datetime module from datetime package
import seaborn as sns  # Import seaborn package

# %% Create some datetime data
dates = [
    datetime(2019, 8, 21),
    datetime(2019, 8, 22),
    datetime(2019, 8, 23),
    datetime(2019, 8, 24),
    datetime(2019, 8, 25),
    datetime(2019, 8, 26),
    datetime(2019, 8, 27),
]

# %% Create a measured variable
Hs = np.random.random_sample(7)

# %% Plot a time series of the "Hs" data
sns.set_theme()  # Set the plotting theme to seaborn style

plt.plot_date(dates, Hs)
plt.tight_layout()
plt.show()
```

2. Run your script in VS code with Ctrl+F5 to test your code.
- Make sure you have your Python environment set correctly; >Python: Set Interpreter —> set it to the datasci environment in VS code.
- Note: Right click > Run in Interactive Window for more functionality (this requires the Jupyter extension for VS code).
  
3. Source Control > Write a message > Commit > Sync Changes

4. Check GitHub online for your changes! 

> You are now a Python Guru with a working Python coding setup 😃

---
