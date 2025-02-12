# Exercises for BIOENG 456: Controlling Behavior in Animals and Robots
Welcome to BIOENG 456: **Co**ntrolling **B**ehavior in **A**nimals and **R**obots (CoBAR)! In this course, we will use [FlyGym](https://github.com/NeLy-EPFL/flygym) to program [NeuroMechFly v2](https://www.nature.com/articles/s41592-024-02497-y) (a digital twin of the adult fruit fly *Drosophila melanogaster*) to interact with the environment and perform complex behaviors.
## Getting started
To begin with the course materials, ensure you have Git, conda, and the FlyGym Python package installed.
### Installing Git
Git is essential for version control and collaboration. Download and install Git from https://git-scm.com/downloads.
### Installing conda
Conda simplifies Python environment management. For a minimal installation, install Conda using Miniconda.

Link to graphical installers:
- Windows: https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe
- macOS (Apple Silicon): https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.pkg
- macOS (Intel-based): https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.pkg

For Linux, refer to the Linux section of https://docs.anaconda.com/free/miniconda/#quick-command-line-install
### Installing FlyGym
Create a Python virtual environment with conda:
```sh
conda create -n flygym python=3.12
```
Activate the environment (run this every time before you use the environment):
```sh
conda activate flygym
```
Clone the flygym repository
```sh
git clone git@github.com:NeLy-EPFL/flygym.git
```
If this fails, try:
```sh
git clone https://github.com/NeLy-EPFL/flygym
```
Bugs and issues may be discovered throughout the semester. The fixes may take time to be merged into the main branch. To ensure you have the latest version, switch to the `cobar` branch.
```sh
cd flygym
git checkout cobar
```
Next, change directory to the cloned repository and install the flygym package in editable mode.
```sh
pip install -e .[dev,examples]
```
On zsh (default shell on MacOs), you need to put [dev,examples] in quotes:
```sh
cd flygym
pip install -e ."[dev,examples]"
```
### Installing Visual Studio Code
- Download and install [Visual Studio Code](https://code.visualstudio.com)
- Open Visual Studio Code and navigate to the Extensions view by clicking on the Extensions icon in the Activity Bar on the left side of the window (or by pressing `Ctrl+Shift+X` on Windows/Linux and `Cmd+Shift+X` on Mac).
- Search for "Python" and install the Python extension provided by Microsoft.
- Search for "Jupyter" and install the Jupyter extension provided by Microsoft.

If you encounter any issues during the installation, feel free to reach out to the TAs.
# Running the notebooks
Open a new terminal and clone this repository:
```sh
git clone https://github.com/NeLy-EPFL/cobar-exercises
```
Open the `cobar-exercises` folder with Visual Studio Code: **File > Open...**

Open the Explorer view in Visual Studio Code by clicking on the Extensions icon in the Activity Bar on the left side of the window (or by pressing `Ctrl+Shift+E` on Windows/Linux and `Cmd+Shift+E` on Mac).

Open one of the .ipynb file within the Explorer view (e.g., `week1/gym_basics_and_kinematic_replay.ipynb`)

Change the kernel to `flygym` (for how to change kernel, refer to https://code.visualstudio.com/docs/datascience/jupyter-kernel-management)

For more instructions on how to work with Jupyter Notebooks in Visual Studio Code, refer to https://code.visualstudio.com/docs/datascience/
jupyter-notebooks.
# Updating the exercises
New exercises will be released every week. Update the repository by:
```sh
cd cobar-exercises
git pull
```
# Updating FlyGym
To update FlyGym, navigate to the FlyGym repository and pull the latest changes:
```sh
cd flygym
git checkout cobar
git pull
```
# Resources
- [FlyGym repository](https://github.com/NeLy-EPFL/flygym/tree/main)
- [FlyGym documentation](https://neuromechfly.org)
- [Setting up git](https://docs.github.com/en/get-started/getting-started-with-git/set-up-git)
# Troubleshooting
If you encounter any issues during the installation or running of the exercises, please reach out to the TAs through the moodle forum.