# Aus Sea Snakes

Welcome to the **Aus Sea Snakes**! 🎉

Aus Sea Snakes are a group of coastal scientists and engineers across Australasia who share Python code, learn together and enhance their programming skills through shared experiences.

## Table of Contents

- [About](#about)
- [Getting Started](#getting-started)
- [Learning Goals](#learning-goals)
- [Getting Help](#getting-help)
- [How to Contribute](#how-to-contribute)
- [Prerequisites](#prerequisites)
- [Code of Conduct](#code-of-conduct)
  

- [Community](#community)
- [License](#license)

## About

The Sea Snakes group is designed for enthusiasts at all levels—from beginners to advanced programmers—to collaborate, share knowledge, and work on exciting Python projects. Whether you're interested in data science, machine learning, coastal modelling or coastal mapping (GIS), there's a place for you here!

## Getting Started

Python is a coding language for scientific programming - a great tool for coastal scientists and engineers to analyse metocean data, create informative graphics and build functions for improved workflows.

“Coding” requires;

- A language: Python in this case,
- A coding environment that stores all the functions and modules used by Python,
- A code editor or interpreter where the user can write, edit and usually run the code (e.g. VS Code, Spyder, IDLE).

### Code setup

In this setup, we use *Anaconda* for managing Python environments and *VS Code (by Microsoft)* for interpreting code. *Black* python package is used to format the code, and *Code Spell Checker* assists programmers in VS code. This setup uses the command prompt (also called terminal) to run some commands for installation (e.g. *conda create —name datasci*).

*Git* is also used here to version control and backing up the code. Github hosts a copy of the code in a repository online (Github account). Here we use github.com/AusSeaSnakes/.github as the homepage to this Sea Snakes group for sharing Python code. *Git* and *Github* are easily integrated into VS code with a pre-installed GitHub extension in VS code.

#### Anaconda installation
1. Download [Anaconda Distribution](https://www.anaconda.com/products/distribution). Anaconda comes with the latest version of Python (no need to install Python directly). Anaconda was designed for scientists in mind and comes with many of the common packages required for scientific programming (e.g. matplotlib for plotting results).
2. Install Anaconda for “Just Me”, not all users, and Add it to your path! - Adding to your path means that you can use it directly from the terminal. Installing for Just Me means you can easily change the virtual environments without Global permissions - great when working on an organisation PC (e.g., university laptop).
3. Your Anaconda folder should have been installed in your “C:\Users\*username*” directory.
4. Check Anaconda (conda) is working by opening a command prompt/terminal and typing “conda”. This should print a long result with something like “conda is a tool for managing and deploying applications, environments and packages.” near the top.

#### Create a virtual environment with Anaconda
'''python
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
'''

### Next steps

1. **Explore the Repositories**: We have repositories for various topics including data science, machine learning, coastal modeling, and more.
2. **Join Discussions**: Each repository has a Discussions section where you can ask questions, share resources, and discuss topics with other members.
3. **Contribute**: Share your code, add to documentation, or take on a new learning challenge! Check out our [Contributing Guidelines](CONTRIBUTING.md) to get started.

## Learning Goals

Our goal is to create a supportive environment for:
- Learning Python fundamentals and advanced concepts
- Building hands-on projects
- Sharing best practices and code snippets
- Collaborating on interesting problems and challenges

## Getting Help

If you have questions about this group or any of the repositories, feel free to reach out in the Discussions tab or open an issue in the relevant repository.

## How to Contribute
We encourage everyone to contribute! Please refer to our Contributing Guidelines for more details.

## Prerequisites

- **Python**: Install Python 3.x from the [official website](https://www.python.org/downloads/)
- **GitHub Account**: If you don't have one, [sign up here](https://github.com/join)

## Code of Conduct

Please read our [Code of Conduct](CODE_OF_CONDUCT.md). We strive to make this a welcoming and friendly place for everyone.

## Community
Join our Discord Server or Slack Workspace to engage with other members, ask questions, and stay updated with the latest activities.

## License
This project is licensed under the [MIT License](LICENSE.md).

Happy coding!

---






