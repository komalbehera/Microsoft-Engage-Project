
# Microsoft-Engage-Project
![ms](https://user-images.githubusercontent.com/58564545/142769147-e13fd821-056c-46fd-b2fb-b62c2eb975d2.png)

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

The Dashboard provides a central interface to all the features of the application. 
The navigation bar has options to signup/login into the web-app; create new forums or join an existing ones. Before being able to post, a user needs to mandatorily login.

### Management Systems

* `Forum System`:
  * Forum creation
  * Replying / posting messages in a forum
  * Forum categories
  * Admin's ability to create forum categories
  * ability to delete your own forum replies 


### Login or Registration and User Authentication

Discussion Forum supports a complete login/registration and User Profile system. On startup, the application shows options for logging in, signing up or contacting the website admin via email. Each user can make a unique username which cannot be changed later. The user `passwords` are `hashed` before storing in database so even admins do not have access to the original passwords as well. Additional User information include `Full Name`, `email`, `Profile Image`, `Profile Headline`, `Gender` and `Bio`.

The app uses several authentication methods for signing up and logging in. It checks for `empty fields`, `wrong username`, `wrong password`, `SQL errors`, `server errors` and in case of signing up, `corrupted image` or `wrong image type` errors

### ChatRoom

Discussion Forum also has a chatbox, which uses `Django` for real-time chatting with other users. A user can access a chat forum by clicking on existing list of forums available , which will retrieve all the chat messages from the database. Chatting is done in real-time, without the need to refresh the page continuously.

**Possible Improvements**:
* `optimization`: All messages of a chat are retrieved at once, and this can cause delays if the chat is big. This can be fixed by implementing incremental load of messages to load only the messages being displayed on-screen.
* `user search`: A search feature can be implemented in the user list to directly search for a particular user, thus saving time.
* `forum search`: A search feature can be implemented in the forums list to directly search for a particular forum, thus saving time.

### Security

* `Password hashing` before storing in database.
* Password Reset done through individually created `encrypted tokens` sent via email as a form of a link. The tokens have a certain expiry date after which they cannot be used.

## Future Improvements
* Optimization (in components like chat room)
* Implementing `Vue.js` for chat room.
* Continuous Bug fixes and improvements

## Screenshots 

homepage:
![home](https://user-images.githubusercontent.com/58564545/143768499-ee32b5b4-9a6e-4387-b826-89f3ecf7fe10.JPG)

signup-page :
![signup](https://user-images.githubusercontent.com/58564545/143768462-13417687-5af7-4736-91d0-3d35feb87b61.JPG)

login-page :
![login](https://user-images.githubusercontent.com/58564545/143768473-a73db4c2-d5db-415f-9da2-aafa61328d5b.JPG)
![after login](https://user-images.githubusercontent.com/58564545/143768491-822c9e4c-fb3d-4371-be34-056eeaeb153d.JPG)

view-groups:
![view groups](https://user-images.githubusercontent.com/58564545/143768521-d6ff089f-d656-40a4-9281-726ebc094d68.JPG)

create-groups:
![create groups](https://user-images.githubusercontent.com/58564545/143768527-b66c0aa7-6c3e-4131-b153-493efcb86c49.JPG)

create-posts:
![create posts](https://user-images.githubusercontent.com/58564545/143768544-5d46fdda-bfa2-4067-9188-4b7c4d6ddc89.JPG)
![eg post](https://user-images.githubusercontent.com/58564545/143768552-8131b761-7f3e-4d61-bf51-62a7d21cfdea.JPG)
![show in group](https://user-images.githubusercontent.com/58564545/143768559-0b5ef3fa-7b45-48e3-9ef7-664e04793384.JPG)

delete-posts:
![delete post](https://user-images.githubusercontent.com/58564545/143768568-9c86eec0-1c60-404c-85f0-8dc063c3a3a3.JPG)

sign-out:
![signout](https://user-images.githubusercontent.com/58564545/143768586-ece155a3-274a-45cc-9f4e-081bbbbe1200.JPG)


## Contributor

Komal Trishna Behera

