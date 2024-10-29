# Linux Setup Guide

This guide provides step-by-step instructions for setting up Python, pip, virtual environments, and Django on a Linux system.

## Prerequisites

Ensure **Python 3** is installed on your system. You can check this by running:

```bash
python3 --version
```



## 1. Install pip3
pip3 is the package manager for Python, allowing you to easily install and manage Python libraries.
```bash
sudo apt update
sudo apt install python3-pip
pip3 --version  # Verify the installation
```




## 2. Install python3-venv
The python3-venv module is used to create isolated Python environments.
```bash
sudo apt update
sudo apt install python3-venv
```



## Create and Activate a Virtual Environment
Create the virtual environment:
```bash
python3 -m venv myenv
```

Activate the virtual environment:
```bash
python3 -m venv myenv
```


## 4. Install Django
Once inside the virtual environment, install Django:
```bash
pip install django
```



## 5. Deactivate the Virtual Environment
To exit the virtual environment, simply run:
```bash
deactivate
```



