
# Microsoft-Engage-Project
![ms](https://user-images.githubusercontent.com/58564545/142769147-e13fd821-056c-46fd-b2fb-b62c2eb975d2.png)
## Setup

The first thing to do is to clone the repository:

```sh
$ git clone https://github.com/komalbehera/Microsoft-Engage-Project.git
```

Create a virtual environment to install dependencies in and activate it:

```sh
$ python -m venv new-env
$ cd new-env/Scripts/activate
```

Then install the dependencies:

```sh
(new-env)$ cd Microsoft-Engage-Project
(new-env)$ pip install -r requirements.txt
```
Note the `(new-env)` in front of the prompt. This indicates that this terminal
session operates in a virtual environment set up by `virtualenv2`.

Once `pip` has finished downloading the dependencies:
```sh
(new-env)$ cd discussion_forum
(new-env)$ python manage.py runserver
```
And navigate to http://127.0.0.1:8000
