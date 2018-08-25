---
layout: post
title: "Starting a simple Django project."
date: 2018-08-26 01:01:20 +0530
description: Djano project setup.
img: # Add image post (optional)
tags: [Tutorial, Django] # add tag
---

# Starting a simple Django project
## Follow these steps one by one
#### 1. First of all install [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/). Follow [instructions on official documentationpage.](https://virtualenvwrapper.readthedocs.io/en/latest/install.html)
#### 2. Once you've installed virtualenvwrapper, create a directory with the name of your project. For example
```shell
$ mkdir demo_app
# then goto the created directory by
$ cd demo_app
```

#### 3. Once you're in your `demo_app` directory, create a virtual environment in the same directory by running following command
```shell
$ mkvirtualenv demo_app -a "$(pwd)" -p python3.6
```

#### 4. Now your virtual environment has been setup. After running the previous command, your virtual env should be activated automatically, if not please run
```shell
$ workon demo_app
```

#### 5. Now you are in your virtual evn. Before we start installing dependecies directly into our virtual environment, it's better to list them first in `requirements.txt` file. Create a file named `requirements.txt` in `demo_app` directory
```shell
$ touch requirements.txt
```

#### 6. In your `requirements.txt` file, you should add the following text:
```text
Django~=2.0.6
```

#### 7. Now, run `pip install -r requirements.txt` to install Django.

#### 8. Once Django is installed, you are ready to start your first Django app. Run the following command
```shell
$ django-admin startproject demo_app .
```

#### 9. Now you should have following file structure
```
.
├── four_chan
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── manage.py
└── requirements.txt
```

#### 10. Now run the initial database migrations via running following command from the directory which contains `manage.py` file
```shell
$ python manage.py migrate
```

#### 11. Finally run `python manage.py migrate` command to start the server
```shell
$ python manage.py runserver
```
# Voila!!! Your project is up and running
![Django Home page]({{site.baseurl}}/assets/img/django.png)

<br>

Link to [GitHub Gist](https://gist.github.com/akashgiricse/efe626272fc7223f41b2140675f598e3)
