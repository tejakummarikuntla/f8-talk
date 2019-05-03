## f8-talk

This repository contains code exercises and materials for facebook-f8 talk on computer vision.
It consists of ipython notebooks that demonstrate various applications and techniques we discussed.
These notebooks depend on a number of software packages to run, and so, we suggest that you create a local environment with these dependencies by following the instructions below.

## 1. Installation

**Download** the latest version of `anaconda` that matches your system.

|        | Linux | Mac | Windows | 
|--------|-------|-----|---------|
| 64-bit | [64-bit (bash installer)][lin64] | [64-bit (bash installer)][mac64] | [64-bit (exe installer)][win64]
| 32-bit | [32-bit (bash installer)][lin32] |  | [32-bit (exe installer)][win32]

[win64]: https://repo.anaconda.com/archive/Anaconda3-2018.12-Windows-x86_64.exe
[win32]: https://repo.anaconda.com/archive/Anaconda3-2018.12-Windows-x86.exe
[mac64]: https://repo.anaconda.com/archive/Anaconda3-2018.12-MacOSX-x86_64.sh
[lin64]: https://repo.anaconda.com/archive/Anaconda3-2018.12-Linux-x86_64.sh
[lin32]: https://repo.anaconda.com/archive/Anaconda3-2018.12-Linux-x86.sh

## 2. Create and Activate the Environment

For Windows users, these following commands need to be executed from the **Anaconda prompt** as opposed to a Windows terminal window. For Mac, a normal terminal window will work. 

#### Git and version control
These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:
```
conda install git
```
**Now, we're ready to create our local environment!**

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two.
```
git clone https://github.com/tejakummarikuntla/f8-talk.git
```

2. Create (and activate) a new environment, named `f8` with Python 3.6. If prompted to proceed with the install `(Proceed [y]/n)` type y.

	- __Linux__ or __Mac__: 
	```
	conda create -n f8 python=3.6
	source activate f8
	```
	- __Windows__: 
	```
	conda create --name f8 python=3.6 
	or
	conda create -n yourenvname python=x.x anaconda
	conda activate f8
	```
3. Install few required packages,
    ```
    > conda install -c conda-forge opencv 
    > conda install -c anaconda numpy 
    > conda install -c conda-forge matplotlib 
    ```
4. That's it!

To exit the environment when you have completed your work session, simply close the terminal window. OR
```
conda deactivate f8
```

