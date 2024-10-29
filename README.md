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



## 3. Create and Activate a Virtual Environment
- Create the virtual environment:
```bash
python3 -m venv myenv
```

- Activate the virtual environment:
```bash
source myenv/bin/activate
```


## 4. Install Django,djangorestframework
Once inside the virtual environment, install Django:
```bash
pip3 install django djangorestframework
```



## 5. Deactivate the Virtual Environment
To exit the virtual environment, simply run:
```bash
deactivate
```


## 6. Django Project Commands
- Create a New Django Project:
```bash
django-admin startproject myproject
```

- Create a New Django App:
```bash
python manage.py startapp myapp
```
- Make Migrations: This command creates migration files for any changes made to the models.
```bash
python manage.py makemigrations
```
- Apply Migrations: This command applies the migration files to the database.
```bash
python manage.py migrate
```
- Create a Superuser: Set up an admin account to access Django’s admin interface.
```bash
python manage.py createsuperuser
```
- Run the Development Server: Start the Django development server to view your project in the browser.
```bash
python manage.py runserver
```
