# Netfix, service marketplace

## Overview

Netfix, service marketplace is a Django-based web application designed to connect service providers with customers in need. Through this platform, users can either offer or request a variety of services, ranging from home cleaning to carpentry. The aim is to create a one-stop solution for individuals to offer and avail different types of home and maintenance services.

![netfix](/img/image2.jpg)

## Tech Stack

- Language: Python
- Framework: Django (v4.2.5)
- Database: SQLite

## Installation

Ensure that you have [Python 4.x](https://www.python.org/downloads/) and [pip](https://pip.pypa.io/en/stable/installation/) installed on your machine. Clone the repository, navigate to the project directory, and install the required packages using the following commands:

```bash
git clone https://learn.zone01dakar.sn/git/mouhamadoufadiop/netfix
cd netfix
```

## Usage

To run the application, execute the following command in the project directory:

```bash
python3 -m venv env 
source env/bin/activate
pip install -r requirements.txt
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver
```

This will start the server on port 8000 by default in virtual environment.
## TestUsers
```
user: test2@gmail.com
mdp : Test2@2024

user: css@gmail.com
mdp : Css@2024

user:miasn@gmail.com
mdp:Miasn@2024

user:ces@gmail.com
mdp:Ces@2024
```

## Features

### Core Features

- User Registration and Login:
  - Customers and Companies can register and login using their email and password.
  - Unique usernames and emails to avoid duplication.
  - Different registration fields for Customers and Companies.

- User Profiles:
  - Profile pages displaying user information.
  - List of requested services for Customers.
  - List of provided services and service creation option for Companies.

- Service Management:
  - Companies can create services based on their field of work.
  - Customers can request services by providing necessary details.
  - Service pages with detailed information and associated Company profile link.
  - Listing of services based on categories, creation time, and popularity.

- Miscellaneous:
  - Navigation bar for easy access to different sections.
  - Logout option for users.

## Structure

The project follows a typical Django project structure, with the main folder housing different apps for handling distinct aspects of the application:

- services: Manages service-related features.
- users: Manages user-related features.
- main: Manages common features across the project.

Each app contains essential Django files like **models.py** for database schema, **views.py** for backend logic, and **urls.py** for routing. Additionally, **forms.py** is used for form handling, and the **templates** directory is used for HTML templates.

Sometimes, there might be multiple virtual environments, and you could be running the wrong one. If virtual environment happens to get corrupted then you can try recreating the virtual environment from scratch.

```
# Deactivate the current virtual environment if it's active
deactivate

# Delete the existing 'env' directory
rm -r env

# Create a new virtual environment
python3 -m venv env

# Activate the new virtual environment
source env/bin/activate

# Reinstall the dependencies
pip install -r requirements.txt

```
## Contributers
- mouhamadoufadiop (Mouhamadou Fadilou Diop)
- [alassall](https://learn.zone01dakar.sn/git/alassall) (Alassane Sall)
