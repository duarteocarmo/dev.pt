<center>
# flask_hackernews <br/>
<a href="https://www.python.org/downloads/release/python-371/">
<img src="https://img.shields.io/badge/python-3.7.1-blue.svg"/></a>
<a href=""><img src="https://img.shields.io/badge/license-MIT-green.svg"/></a>
<a href="https://heroku.com"><img src="https://img.shields.io/badge/deploy-heroku-purple.svg"/></a>
<a href="https://github.com/ambv/black"><img src="https://img.shields.io/badge/style-black-black.svg"/></a>
<a href="http://flask.pocoo.org/"><img src="http://flask.pocoo.org/static/badges/flask-project-s.png"/></a>
</br>
</center>
**flask_hackernews** is a minimalistic [hackernews](new.ycombinator.com) clone. 

This was built so that beginners who want a hackernews-like application can quickly get to work. 

Greatly inspired by the awesome [flask megatutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world).

We use: 

- `flask` as a web framework.
- `flask-sqlalchemy` as an ORM.
- `SQLite` as a database.
- `heroku` for a simple deployment.
- Some other goodies 😉 (check `requirements.txt`)

And that's pretty much it!

### Contents

- [Features](#Features)
- [Set up](#SetupInstructions)
- [Deployment](#Deployment)
- [About](#About)


### Features
- user authentication
- upvoting on comments and posts
- karma
- user profiles
- post ranking algorithms based on the ['official'](https://news.ycombinator.com/item?id=1781417) one
- comment replies, threading and more!

### Set up Instructions

*Follow these instructions if you wish to run this project locally*

- clone this repo

```bash
$ git clone https://github.com/duarteocarmo/flask_hackernews
```

- create a virtual environment with the latest python version
- install requirements

```bash
(venv) $ pip install -r requirements.txt
```

- create a `.env` file in the home directory with the following structure

```python
FLASK_APP=flasknews.py
SECRET_KEY = "yoursecretkey"
MAIL_ADMIN_ADDRESS = <admin_email_adress>
MAIL_SERVER = <admin_mail_server>
MAIL_PORT = <admin_mail_port>
MAIL_USE_TLS = 1
MAIL_USERNAME = <admin_email_adress>
MAIL_PASSWORD = <admin_email_password>
```



- initiate your database

```bash
(venv) $ flask db init
(venv) $ flask db upgrade
```

- 🎉Run!!🎉

```bash
(venv) $ flask run
```

- visit [`http://localhost:5000`](http://localhost:5000) to check it out.

### Deployment

*Follow these instructions to deploy your to the 🌎*

- Heroku: follow [this guide](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-xviii-deployment-on-heroku).
- Docker: follow [this guide](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-xix-deployment-on-docker-containers).
- Linux: follow [this guide](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-xvii-deployment-on-linux).


### About

This project was built by duarteocarmo. If you have any questions, [contact me](https://duarteocarmo.com)!