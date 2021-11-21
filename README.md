[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Apurva-tech/unite?logo=github&style=for-the-badge)](https://github.com/Apurva-tech/) 
[![GitHub last commit](https://img.shields.io/github/last-commit/Apurva-tech/unite?style=for-the-badge&logo=git)](https://github.com/Apurva-tech/) 
[![GitHub stars](https://img.shields.io/github/stars/Apurva-tech/unite?style=for-the-badge)](https://github.com/Apurva-tech/unite/stargazers) 
[![My stars](https://img.shields.io/github/stars/Apurva-tech?affiliations=OWNER%2CCOLLABORATOR&style=for-the-badge&label=My%20stars)](https://github.com/Apurva-tech/unite/stargazers) 
[![GitHub forks](https://img.shields.io/github/forks/Apurva-tech/unite?style=for-the-badge&logo=git)](https://github.com/Apurva-tech/unite/network)
[![Code size](https://img.shields.io/github/languages/code-size/Apurva-tech/unite?style=for-the-badge)](https://github.com/Apurva-tech/unite)
[![Languages](https://img.shields.io/github/languages/count/Apurva-tech/unite?style=for-the-badge)](https://github.com/Apurva-tech/unite)
[![Top](https://img.shields.io/github/languages/top/Apurva-tech/unite?style=for-the-badge&label=Top%20Languages)](https://github.com/Apurva-tech/unite)
[![Issues](https://img.shields.io/github/issues/Apurva-tech/unite?style=for-the-badge&label=Issues)](https://github.com/Apurva-tech/unite)
[![Watchers](	https://img.shields.io/github/watchers/Apurva-tech/unite?label=Watch&style=for-the-badge)](https://github.com/Apurva-tech/unite/) 

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
