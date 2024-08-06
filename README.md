### Getting started with your computing environment

## What is conda? What is Miniconda?
Conda is an open-source, cross-platform, language-agnostic package management system 
that also supports environment management. It was created by Continuum Analytics 
(now Anaconda, Inc.) and is included in both the Anaconda and Miniconda distributions.

Conda allows you to install packages from various repositories, manage these packages, 
and also manage environments, which are isolated spaces where packages can be installed 
without interfering with each other. This is particularly useful in the case where 
different projects have conflicting dependencies.

Miniconda, on the other hand, is a minimalist distribution of the Anaconda 
Python distribution. It comes with Python, Conda, and only a handful of other 
basic packages pre-installed. Unlike the full Anaconda distribution, which includes 
over 200 scientific packages and their dependencies, Miniconda is a lightweight 
version intended for users who want more control over their Python environment and are 
willing to manually install the packages they need.

It is recommended to use Miniconda.

## Miniconda installation

We we use the CLI (command line interface) to install Miniconda. 

First, we need to update and upgrade:
```
sudo apt-get update && sudo apt-get upgrade -y
```

Next, make sure we have wget installed:
```
sudo apt-get install wget
```

Then, we need to pull down the latest version of Miniconda and install with our shell:
* For Linux
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh \\
$SHELL Miniconda3-latest-Linux-x86_64.sh
```
* For MacOS Intel
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh \\
$SHELL Miniconda3-latest-MacOSX-x86_64.sh
```
* For MacOS M1
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh \\
$SHELL Miniconda3-latest-MacOSX-arm64.sh
```
* For Windows
Not yet documented.

Follow the instructions to install Miniconda. You may need to source your shell configuration file. This will change depending on your shell, however it will look something like
```
source ~/.bashrc
```

## Now you can create an environment specifically for your AI/ML projects.


## Recommended development environment

As we begin to build AI / ML projects, it's important to set ourselves up to be able to scale successfully. Generally, your projects will contain three components, so it's recommended to set up your directory structure as follows:

/home/{username}/
├─ documents/
│  ├─ code/
│  ├─ data/
│  ├─ results/

