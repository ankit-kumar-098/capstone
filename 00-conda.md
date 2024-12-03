# Installing Miniconda
Miniconda is a minimal installer for Conda, Python, their dependencies and a small collection of packages. Conda itself fulfills two functions:
1. Conda is a package manager, i.e. think of it as an App Store where you can get apps for the command-line interface (CLI). These apps are downloaded as so-called packages.
2. Conda acts as an environment manager. One of the difficulties when working with software tools is that these often have dependencies, i.e. need other programs to properly function (which might themselves need other programs and so on). Unfortunately, some programs might, at the same time, conflict with other programs or only work with specific version numbers. It is often difficult to have one universal install in which all of the tools will work predictably at the same time. Instead, an environment manager enables you to configure independent environments, i.e. a set of programs (each also with a defined version) in which one tool or combination of tools works.
The installation instructions below assume that you have already set up `bash` on macOS or Linux systems or, if you are on a Windows machine, installed the Windows Subsystem for Linux (WSL).

Steps:
- In the Terminal (on Windows, switch to WSL), download the Miniconda installer
```{bash}
curl -sL \
  "https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh" > \
  "Miniconda3.sh"
```
- Install Miniconda by entering and follow the prompts, accepting all defaults.
```{bash}
bash Miniconda.sh
```
- Source the `.bashrc` file:
```{bash}
source ~/.bashrc
```
- Update Conda using the command
```{bash}
conda update conda
```
- After installation, delete the installer:
```{bash}
rm Miniconda.sh
```