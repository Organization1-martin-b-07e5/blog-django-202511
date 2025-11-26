# blog-django-202511

## Requirements

My versions:

```bash
$ python --version  # Python 3.13.5
$ pip --version     # pip 25.1.1
```

---

## Project Setup

### 01 - Clone the Repository

```bash
$ git clone https://github.com/Organization1-martin-b-07e5/blog-django-202511.git
```

---

### 02 - Create a Virtual Environment within the project directory by typing

```bash
$ python -m venv env && echo ok || echo error
```

This will create the `env` directory containing a copy of the Python interpreter and various supporting files.

---

### 03 - Activate the Virtual Environment

```bash
(linux) $ source ./env/bin/activate
(windows) $ ./env/Scripts/activate
```

Example:

```bash
(env) ➜  blog-django-202511 git:(feature/update-readme) pwd
$HOME/django/2025/blog-django-202511
```

---

### 04 - Upgrade PIP

Check the current version:
```bash
BEFORE
(env) $ pip freeze
returns nothing
```

```bash
(env) $ pip list
```

Upgrade to the latest version:

```bash
(linux) (env)   $ pip install -U pip && echo "👈❗DO NOT run this line in Win"
(windows) (env) $ ./env/Scripts/python.exe -m pip install --upgrade pip && echo ok
```

After upgrade:

```bash
(env) ➜  pip --version
pip 25.3 from $HOME/django/2025/blog-django-202511/env/lib/python3.13/site-packages/pip (python 3.13)
```

---

### 05 - Install Django (If not cloned with it)

```bash
(env) ➜  blog-django-202511 git:(feature/update-readme) pip install -U Django
```

Check installed packages:

```bash
(env) ➜  blog-django-202511 git:(feature/update-readme) pip list
```

---

### 06 - Create `requirements.txt`

If not cloned with the repo, create the requirements file:

```bash
$ pip freeze > requirements.txt
```

---

### 07 - Install Requirements

```bash
(env) $ pip install -r ./requirements.txt && echo option1_ok
(env) $ python -m pip install -r ./requirements.txt && echo option2_ok
```

---

### 08 - Create the New Project

```bash
(env) $ django-admin startproject blogName
```

Change to project directory:

```bash
(env) $ cd blogName
```

Check for potential issues:

```bash
(env) ➜  blog git:(feature/update-readme) ✗ ./manage.py check
System check identified no issues (0 silenced).
```

---

### 09 - Create a Django Admin User

If you encounter an error, run `makemigrations` and then `migrate` first:

```bash
(linux) (env) $ ./manage.py createsuperuser
(windows) (env) $ python manage.py createsuperuser
```

Example user details:

```
usr: admin
pass: q1w2e3

usr: grupo3
pass: q1w2e3
```

---

### 10 - Change a User's Password

```bash
(linux) (env) $ ./manage.py changepassword yourUserName
(windows) (env) $ python manage.py changepassword yourUserName
```

---

### 11 - Start the Server on a Different Port

```bash
(env) ➜  blog git:(feature/update-readme) ✗ ./manage.py runserver localhost:8081
```
