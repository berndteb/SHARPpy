# SHARPpy

###### Sounding/Hodograph Analysis and Research Program in Python

[![Test Status](https://github.com/NUCAPS/SHARPpy/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/NUCAPS/SHARPpy/actions/workflows/pytest.yml)
[![Build Status](https://github.com/NUCAPS/SHARPpy/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/NUCAPS/SHARPpy/actions/workflows/build.yml)
[![Anaconda-Server Badge](https://anaconda.org/conda-forge/sharppy/badges/downloads.svg)](https://anaconda.org/conda-forge/sharppy)
[![Anaconda-Server Badge](https://anaconda.org/conda-forge/sharppy/badges/license.svg)](https://anaconda.org/conda-forge/sharppy)
[![](https://img.shields.io/github/downloads/sharppy/SHARPpy/total.svg?style=popout)](https://github.com/sharppy/SHARPpy/releases)
[![Coverage Status](https://coveralls.io/repos/github/sharppy/SHARPpy/badge.svg?branch=master)](https://coveralls.io/github/sharppy/SHARPpy?branch=master)
[![Anaconda-Server Badge](https://anaconda.org/conda-forge/sharppy/badges/platforms.svg)](https://anaconda.org/conda-forge/sharppy)

SHARPpy is a collection of open source sounding and hodograph analysis routines, a sounding plotting package, and an interactive, __cross-platform__ application for analyzing real-time soundings all written in Python. It was developed to provide the atmospheric science community a free and consistent source of sounding analysis routines. SHARPpy is constantly updated and vetted by professional meteorologists and climatologists within the scientific community to help maintain a standard source of sounding routines.

### Important links:
* [User Guide](http://sharppy.github.io/SHARPpy/index.html)
* [BAMS article](https://journals.ametsoc.org/view/journals/bams/98/8/bams-d-15-00309.1.xml)
* [Installation Guide](https://sharppy.github.io/SHARPpy/install.html)

**Table of Contents**
- [Easy install using executable files](#easy-sharppy-using-executable-files)
- [Regular install using Python](#regular-install)
  - [Pre-requisites](#pre-requisites)
  - [Install options](#install-options)
  - [Running SHARPpy from the command line](#running-sharppy-from-the-command-line)
- [SHARPpy Development Team](#sharppy-development-team)

***

## Easy SHARPpy using executable files
<sup>[[Return to Top]](#sharppy)</sup>

If you are using Windows or a Macintosh, SHARPpy is available as a pre-compiled executable file! Click on the [releases section](https://github.com/sharppy/SHARPpy/releases) on the right and select the latest version of SHARPpy. Under assets, you can select the zip file for you operating system. You can unzip and run SHARPpy by double clicking on the SHARPpy.exe (windows) or SHARPpy (mac).

Note: You may need administrative permissions to run executables on your machine, so please consult with your IT department if you have problems.

***

## Regular install
<sup>[[Return to Top]](#sharppy)</sup>

Use this option if you are unable to run executable files or you are interested in using the scripting features.

### Pre-requisites

You will need Python 3 to run SHARPpy. For instructions, visit the following websites:
* https://www.anaconda.com/products/individual for instructions on how to set-up Python.

You will need run a few simple commands in a command line program:
* Linux/MacOS: Open the Terminal application.
* Windows: Open the Anaconda Prompt application.

Note: If you are installing Anaconda for **multiple users**, [ensure these additional steps are met](https://docs.anaconda.com/anaconda/install/multi-user/), which includes checking the permissions using an administrator account.

### Install options
First, you must download the SHARPpy package to your computer. We show different options to accommodate different user and system needs.

#### Option 1: conda forge (easiest)
<sup>[[Return to Top]](#sharppy)</sup>

Open the command line (Anaconda Prompt on Windows, Terminal on MacOs/Linux) type the following command:

```bash
conda install -c conda-forge sharppy
```
This will download and install SHARPpy. Skip to the [running SHARPpy from the command line](#running-sharppy-from-the-command-line) section.

#### Option 2: Manual download (easy)

You can manually download the SHARPpy package by clicking the "Code" button at the top right of the repository, then select "Download Zip." Unzip the files in the directory that you want to permanently store them.

Skip to the [Install SHARPpy from the Command Line](#install-sharppy-from-the-command-line) section.

#### Option 3: Download using Git (intermediate)

If you have Git installed and are familiar with it, open the command line for your operating system (see above) to perform these steps.

```bash
git clone https://github.com/sharppy/SHARPpy
```
Skip to the [Install SHARPpy from the Command Line](#install-sharppy-from-the-command-line) section.

### Install SHARPpy from the command line

If you did option 1 above, you can skip to the next section. If you did option 2 or 3, open the terminal (UNIX/Linux) or Anaconda Prompt (Windows) and change your directory to where you have downloaded SHARPpy (e.g. /home/{user}/SHARPpy).

```bash
cd /home/<user>/SHARPpy
```

Next, we to create an isolated Anaconda environment just for running SHARPpy with all the necessary libraries (using conda env create {options}; it may take several minutes to install the libraries). If you are interested, you can open the environment.yml file to see which libraries are used.

```bash
conda env create -f environment.yml
```

After creating the environment, we need to switch to this new environment (via conda activate {env_name}) which we have named devel.

```bash
conda activate devel
```

Run setup.py to update SHARPpy.

```bash
python setup.py install
```

Once the installation is complete, keep the terminal open and follow the steps in the next section to launch SHARPpy.

### Running SHARPpy from the command line

In the command line, type the command sharppy to launch the program.

```bash
sharppy
```

If successful, a window will open which will give you access to soundings from RAOBS, select models, and NUCAPS.

### How to run SHARPpy next time you log on

If you close the terminal window, you will have to repeat the following steps:

1. Open the terminal (Unix/Linux) or Anaconda Prompt (Windows)
2. Switch your environment to devel ("conda activate devel") [note: skip if you did option 1]
3. Type sharppy and the window should launch.

```bash
conda activate devel
sharppy
```

***

## SHARPpy Development Team
<sup>[[Return to Top]](#sharppy)</sup>

SHARPpy is currently managed by the following co-developers (in no particular order):

- Patrick Marsh (SPC)
- Kelton Halbert (SPC)
- Greg Blumberg (Millersville University)
- Tim Supinie (Center for Analysis and Prediction of Storms)
- Rebekah Esmaili (Science and Technology Corp.)
- Jeff Szkodzinski (Science and Technology Corp.)

If you are interested in providing feedback or contributing, checkout [our guide](https://sharppy.github.io/SHARPpy/contributing.html) for some tips!
