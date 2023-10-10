# ML4DQM PODAS Exercise
A repository to host the Tracker DQM ML exercise for CMS PO DAS.

### Exercise 1 (`exercise1.ipynb`):
This is a tutorial covering the following topics:
- Where to find input data suitable for DQM/DC machine learning studies and how to read and prepare it.
- How to train and evaluate an autoencoder model to spot anomalous lumisections.

Note: this is the version of the exercise compatible with SWAN (lxplus) at CERN. It will not work on the DESY NAF system because of different installed python modules and paths to input files. For the fully PODAS compatible version, see the `desy-podas` branch [here](https://github.com/CMSTrackerDPG/ML4DQMPODASExercise/tree/desy-podas).

How to get this notebook running:

- Open a terminal and connect to lxplus (as follows: `ssh -X <username>@lxplus.cern.ch`).
- Navigate to your `eos` home directory: `/eos/user/<initial>/<username>` (e.g. for the account `llambrec` that would be `/eos/user/l/llambrec`).
- Clone this repository (the main branch) in your `eos` home directory. You can do this as follows in the terminal: `git clone https://github.com/CMSTrackerDPG/ML4DQMPODASExercise.git`.
- Open a SWAN session [here](https://swan.cern.ch/). You can leave all options at the standard settings.
- In SWAN, go to `CERNBox`, then `ML4DQMPODASExercise`. Open the exercise notebook from the SWAN session. There are a few further steps, explained in the notebook itself but repeated below.
- There is one dedicated repository with useful tools that you will need to install manually, namely [this one](https://github.com/LukaLambrecht/ML4DQMDC-PixelAE). Clone it to your DESY workspace (as follows: `git clone https://github.com/LukaLambrecht/ML4DQMDC-PixelAE`). Then modify the path in the first notebook code cell to wherever you downloaded the repository in order for all the imports later on in the script to work. If you downloaded both repositories in your `eos` home directory, you don't have to change anything.
