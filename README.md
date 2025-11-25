# blog-django-202511

```
$ python --version
$ pip3 --version

eg:
➜  blog-django-202511 git:(feature/update-readme) python --version
Python 3.13.5
➜  blog-django-202511 git:(feature/update-readme) pip --version
pip 25.1.1 from /usr/lib/python3/dist-packages/pip (python 3.13)
```

---

✅✍01-07. Create a new folder dedicated to the project or clone it.

Now, whenever you start a new project, you can create a virtual environment for it.

    $ git clone https://github.com/Organization1-martin-b-07e5/blog-django-202511.git

---

✅✍02-07. Create a virtual environment within the project directory by typing:

    $ python -m venv env && echo ok || echo error

👀 This will create the env directory if it doesn’t exist, and also create directories inside it
containing a copy of the Python interpreter and various supporting files.

---

✅✍✍03-07. Once you’ve created a virtual environment, you may ACTIVATE it.

    (linux) $ source ./env/bin/activate
    (win11) $ source ./env/Scripts/activate

[Virtual Environments and Packages¶](https://docs.python.org/3/tutorial/venv.html)

```eg:
➜ blog-django-202511 git:(feature/update-readme) source ./env/bin/activate
(env) ➜ blog-django-202511 git:(feature/update-readme) pwd
$HOME/django/2025/blog-django-202511
```

---
