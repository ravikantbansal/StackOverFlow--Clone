## StackOver Flow - Clone

<a href="https://github.com/Yawan-1/StackOverFlow--Clone/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/Yawan-1/StackOverFlow--Clone"></a>
<a href="https://github.com/Yawan-1/StackOverFlow--Clone/blob/master/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/Yawan-1/StackOverFlow--Clone"></a>
<img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/m/Yawan-1/StackOverFlow--Clone">
![python3.x](https://img.shields.io/badge/python-3.x-brightgreen.svg)

Thanks to Yawan for this great development.

## Images

<img src="/images/animation.gif">

## Demo


## Technology Stack

* [Python 3.7.x](https://www.python.org/)
* [Django Web Framework 3.2.x](https://www.djangoproject.com/)
* [Redis 5.x](https://pypi.org/project/django-redis/)
* [BootStrap 4](https://getbootstrap.com/)
* [Jquery 3](https://api.jquery.com/)
* [Postgresql 14](https://www.postgresql.org/)


## Functionalities


* 50+ Badges are implemented to award
* 20 Privileges to Earn
* Track Badges
* Reputation Awarding
* Privilege and Activity Notifications
* Live Q&A MarkDown Preview
* User @mentioning in comments
* Create and award Bounties
* <code>Threading</code> to keep track of the remaining days of Bounty.
* Reviewing Tasks :
  * First Question Review
  * First Answer Review
  * Late Answer Review
  * Review Flag Posts
  * Review Flag Comments
  * Review Close Votes
  * Review ReOpen Votes
  * Review Low-Quality Posts
  * Review Suggested Edits


* And much more. You can find list of all functionalities <a href="https://github.com/Yawan-1/StackOverFlow--Clone/blob/759157fc68f59398d9352ddd705eee396336bb81/Functionalities.md">Here</a>


## Setup Commands

Clone this repository

1. Clone this project using
````
$ git clone https://github.com/Yawan-1/StackOverFlow--Clone
````

For Postgresql usage*, you will need to download and install it.

1. Download Postgresql from [this Link](https://www.postgresql.org/download/)
2. After installation, create Database in postgresql shell using these commands
   1. `CREATE DATABASE so_clone;`
   2. `CREATE USER so_clone_user WITH PASSWORD 'password';`
   3. `GRANT ALL PRIVILEGES ON DATABASE so_clone TO so_clone_user;`
3. and fill **database name** , **database password** and **user** in `settings.py` like

  ````
  DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'so_clone',
        'USER': 'so_clone_user',
        'PASSWORD': 'password',
        'HOST': 'localhost',
        'PORT': '',
    }
}
  ````

_*Note: You can skip postgresql installation if you're setting up this project using sqlite. simply just comment the postgresql configuration and uncomment sqlite configuration_



Now run make <code>migrations</code> command, running make migrations command will perform Data Migrations to save the "Badges" in the database.
then migrate to load the operations of Data Migrations in database.
````
$ python manage.py makemigrations
$ python manage.py migrate
````

Then, simply run the server using this command.
````
$ python manage.py runserver
````

## Deployment

The following details and steps on how to deploy this application

#### Heroku

See detailed [Deploying django app on Heroku](https://devcenter.heroku.com/articles/django-app-configuration)

Prerequisites
To start with, there are few prerequisites needed before your website goes viral on the internet. There are two pieces of software that need to be installed on your PC to help you deploy the app.

Git — Git is a version control tool that enables you to push and commit new changes to your codebase while preserving the previous versions. It's good practice to use Git for managing your project. To install Git, you can download it from the link provided, based on your OS — https://git-scm.com/downloads

Heroku CLI — Heroku CLI is the Heroku client application, which is used to push your code to the Heroku web server. You will need to download the Heroku CLI and set it up with Git on your PC. This has been explained wonderfully on Heroku CLI website. Here is the link for the same — https://devcenter.heroku.com/articles/heroku-cli

Heroku Login — Another requirement is that you will have to create a Heroku account. This can be made on https://www.heroku.com

Python Virtual Environment — The next requirement is python virtual environment setup. Python virtual environment creates an environment for your project, within which you can install the dependencies which only that project requires. This helps you install only those dependencies on the cloud and save up space. To install Python Virtual environment, just run pip install virtualenv. Here is the link for the same — https://pypi.org/project/virtualenv/

## Contributing

If you have any question or issues, It may have bugs that i may have missed. You can create <a href="https://github.com/Yawan-1/StackOverFlow--Clone/pulls">Pull request</a> or you can also contact me.



