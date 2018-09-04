# Mischung
Telegram bot for testing anything

----------------------------------------------------------------------
### Setting up Git for GitHub:
```
ssh-keygen -t rsa -b 4096 -C "your_mail@example.com"
ssh-add ~/.ssh/your_key_name
```
<https://github.com/settings/keys>
```
git init
git remote add Mischung git@github.com:Artyom-Barsov/Mischung.git
git pull
```
----------------------------------------------------------------------
### Setting up for Heroku:
- Instal heroku
- Login on Heroku
- In Pipfile version:
```
[requires]
python_version = "3.5"
```
- Create Pipfile.lock:
```
pipenv lock
```
- In Procfile how to run:
```
web: python3 bot.py
```
- In requirements.txt are libraries.

```
heroku login
heroku git:remote -a app_name
heroku buildpacks:set heroku/python
heroku ps:scale web=1
heroku maintenance:off
heroku open
```
----------------------------------------------------------------------
### To GitHub:
```
git add .
git commit -am "commit on GitHub"
git push Mischung master
```
Automatic deploys to Heroku can be set up

----------------------------------------------------------------------
### To Heroku:
```
git add .
git commit -am "commit on Heroku"
git push heroku master
```
