
# Microsoft-Engage-Project
![ms](https://user-images.githubusercontent.com/58564545/142769147-e13fd821-056c-46fd-b2fb-b62c2eb975d2.png)

<p align="center">
  <img src="_git%20assets/cover.png" width="600" align="center"/>
</p>

A Django based Discussion Forum web-app.
# Table of Contents

* [Installation](#installation)
  * [Requirements](#requirements)
  * [Setup](#Setup)
* [Features](#Features)
* [Components](#Components)
  * [Languages](#Languages)
  * [Development Environment](#Development-Environment)
  * [Database](#database)
  * [Frameworks and Libraries](#Frameworks-and-Libraries)
  * [Techniques](#techniques)
* [Details](#details)
* [Future Improvements](#future-improvements)
* [Contributor](#Contributor)



## Installation

#### Requirements
* Django
* SQLite Database

#### Installation Steps
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


## Features

* [Application Dashboard](#application-Dashboard)
* [Login/Registration and User Authentication](#Login-or-Registration-and-User-Authentication)
* [Inbox/Chat room](#chatroom)
* [Forum system](#management-systems)
* [Blog Management system](#management-systems)
* [Security](#security)


## Components

#### Languages
```
Django 1.11.17
JavaScript ES 6
HTML5
CSS3
Bootstrap3
```

#### Development Environment
```
Windows 10
```

#### Database
```
SQLite 3.31.1
```


#### Frameworks and Libraries
```
JQuery v3.3.1
BootStrap v4.2.1
```

#### Techniques
```
Web Socket
```

## Details

> Details of important Features of the Application

### Application Dashboard

<p align='center'>
  <img src="_git%20assets/dashboard.png" width="500" align="center"/>
</p>

The Dashboard provides a central interface to all the features of the application. 
The navigation bar has options to signup/login into the web-app; create new forums or join an existing ones. Before being able to post, a user needs to mandatorily login.

### Management Systems

<p align="center">
  <img src="_git%20assets/management.png" width="600" align="center"/>
</p>

* `Forum System`:
  * Forum creation
  * Replying / posting messages in a forum
  * Forum categories
  * Admin's ability to create forum categories
  * ability to delete your own forum replies 


### Login or Registration and User Authentication

<p>
  <img src="_git%20assets/login.png" width="400" align="right"/>
</p>

Discussion Forum supports a complete login/registration and User Profile system. On startup, the application shows options for logging in, signing up or contacting the website admin via email. Each user can make a unique username which cannot be changed later. The user `passwords` are `hashed` before storing in database so even admins do not have access to the original passwords as well. Additional User information include `Full Name`, `email`, `Profile Image`, `Profile Headline`, `Gender` and `Bio`.

The app uses several authentication methods for signing up and logging in. It checks for `empty fields`, `wrong username`, `wrong password`, `SQL errors`, `server errors` and in case of signing up, `corrupted image` or `wrong image type` errors

### ChatRoom

<p align="center">
  <img src="_git%20assets/inbox.png" width="600" align="center"/>
</p>

Discussion Forum also has a chatbox, which uses `Django` for real-time chatting with other users. A user can access a chat forum by clicking on existing list of forums available , which will retrieve all the chat messages from the database. Chatting is done in real-time, without the need to refresh the page continuously.

**Possible Improvements**:
* `optimization`: All messages of a chat are retrieved at once, and this can cause delays if the chat is big. This can be fixed by implementing incremental load of messages to load only the messages being displayed on-screen.
* `user search`: A search feature can be implemented in the user list to directly search for a particular user, thus saving time.
* `forum search`: A search feature can be implemented in the forums list to directly search for a particular forum, thus saving time.

### Security

* `Password hashing` before storing in database.
* Password Reset done through individually created `encrypted tokens` sent via email as a form of a link. The tokens have a certain expiry date after which they cannot be used.
* 
## Future Improvements
* Optimization (in components like chat room)
* Implementing `Vue.js` for chat room.
* Continuous Bug fixes and improvements

## Contributor

Komal Trishna Behera

