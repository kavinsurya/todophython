## Setup

- Run `pipenv install`

## Run Dev Server

- Run `pipenv shell` once
- Then run `python main.py`

## Hosting

- `git init` first
- `git add .` and `git commit -am "First Commit"`
- Run the command given in the heroku page `heroke remote ...`
- Create a `Procfile` for Heroku as heroku does not support flask run by default.
- `web: gunicorn main:app` Paste this in the Procfile. 
-`web` is used by Heroku to know which command to run.
- `gunicorn` is a python process manager.
- `main:app` tells gunicorn to run app module from the main.py file.
- Finally, `git push heroku master`