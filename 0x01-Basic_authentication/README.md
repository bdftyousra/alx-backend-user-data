# 0x06. Basic authentication
:open_file_folder: Specializations - Web Stack programming ― Back-end  
:bust_in_silhouette: by Guillaume, CTO at Holberton School  
:copyright: **[Holberton School](https://www.holbertonschool.com/)**  
:bookmark:

## Background Context
In this project, you will learn what the authentication process means and implement a Basic Authentication on a simple API.

## Resources
### Read or watch:
* [REST API Authentication Mechanisms](https://www.youtube.com/watch?v=501dpx2IjGY)
* [Base64 in Python](https://docs.python.org/3.7/library/base64.html)
* [HTTP header Authorization](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Authorization)
* [Flask](https://palletsprojects.com/p/flask/)
* [Base64 - concept](https://en.wikipedia.org/wiki/Base64)
* [Custom Error Pages](https://flask.palletsprojects.com/en/1.1.x/patterns/errorpages/)
* [before_request](https://flask.palletsprojects.com/en/1.1.x/api/#flask.Blueprint.before_request)
* [Download and start your project from this archive](https://intranet.hbtn.io/rltoken/scy2k-OPTBy-DI90EyQ0uw)
# Simple API

Simple HTTP API for playing with `User` model.


## Files

### `models/`

- `base.py`: base of all models of the API - handle serialization to file
- `user.py`: user model

### `api/v1`

- `app.py`: entry point of the API
- `views/index.py`: basic endpoints of the API: `/status` and `/stats`
- `views/users.py`: all users endpoints


## Setup

```
$ pip3 install -r requirements.txt
```


## Run

```
$ API_HOST=0.0.0.0 API_PORT=5000 python3 -m api.v1.app
```


## Routes

- `GET /api/v1/status`: returns the status of the API
- `GET /api/v1/stats`: returns some stats of the API
- `GET /api/v1/users`: returns the list of users
- `GET /api/v1/users/:id`: returns an user based on the ID
- `DELETE /api/v1/users/:id`: deletes an user based on the ID
- `POST /api/v1/users`: creates a new user (JSON parameters: `email`, `password`, `last_name` (optional) and `first_name` (optional))
- `PUT /api/v1/users/:id`: updates an user based on the ID (JSON parameters: `last_name` and `first_name`)

## Learning Objectives
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/2012/04/feynman-technique/), without the help of Google:
### General
* What authentication means
* What Base64 is
* How to encode a string in Base64
* What Basic authentication means
* How to send the Authorization header

## Requirements
* A ```README.md``` file.

## Tasks
* [x] 0. Simple-basic-API
* [x] 1. Error handler: Unauthorized
* [x] 2. Error handler: Forbidden
* [x] 3. Auth class
* [x] 4. Define which routes don't need authentication
* [x] 5. Request validation!
* [x] 6. Basic auth
* [x] 7. Basic - Base64 part
* [x] 8. Basic - Base64 decode
* [x] 9. Basic - User credentials
* [x] 10. Basic - User object
* [x] 11. Basic - Overload current_user - and BOOM!
* [x] 12. Basic - Allow password with ":"
* [x] 13. Require auth with stars

## Software engineer
Javier Andrés Garzón Patarroyo  
:octocat: [GitHub](https://github.com/javierandresgp/)
