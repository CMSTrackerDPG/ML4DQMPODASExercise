# ML4DQM PODAS Exercise
A repository to host the Tracker DQM machine learning exercises for the CMS PO DAS school at DESY, October 2023.

### Exercise 1 (`exercise1.ipynb`):
This is a tutorial covering the following topics:
- Where to find input data suitable for DQM/DC machine learning studies and how to read and prepare it.
- How to train and evaluate an autoencoder model to spot anomalous lumisections.

How to get this notebook running:  
- Open a terminal and connect to the DESY system with the account you received (e.g. ssh schoolXX@naf-cms.desy.de).
- Clone this repository [here](https://github.com/CMSTrackerDPG/ML4DQMPODASExercise/tree/desy-podas) in your DESY workspace. Make sure to have the `desy-podas` branch, not the `main` branch.
- Open a DESY JupyterHub session [here](https://naf-jhub.desy.de/hub/spawn). Log in with your received account, select CMS for Primary Group, the rest can be left at default, or use JupyterLab mode instead of Classical Notebook mode if you prefer. It can take 30 seconds for the session to start.
- Open the exercise notebook from the JupyterHub session. There are a few further steps, explained in the notebook itself but repeated below.
- There is one dedicated repository with useful tools that you will need to install manually, namely [this one](https://github.com/LukaLambrecht/ML4DQMDC-PixelAE). Clone it to your DESY workspace. Then modify the path in the first notebook code cell to wherever you downloaded the repository in order for all the imports later on in the script to work.
- For all other dependencies, we prepared a virtual environment that contains all of them. The steps below show how to activate it.
- In your terminal, enter the following command: `source /nfs/dust/cms/group/cmsdas2023/TRK-DQM/venv_ml4dqm_podas2023/bin/activate` to activate the virtual environment in that terminal.
- Next, run this command: `ipython kernel install --user --name=venv_ml4dqm_podas2023` to register the environment as an ipython kernel.
- Finally, in the JupyterHub (where you have the notebook open), go to Kernel -> Change kernel... and select the kernel named `venv_ml4dqm_podas2023`. (Potentially you need to refresh the page first).
