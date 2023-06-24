# Flask Setup

## Prerequisites

To install Flask, you'll need:
- Python
- pip (comes with Python)
- A Terminal application
  - For windows, we [recommend Cmder](windows-setup-guide.md)
  - For Mac, we [recommend Iterm2](macos-setup-guide.md)
  - Alternatively, use the terminal built into VSCode

## Install Flask

1. Open your terminal application (probably Cmder or Iterm2).
2. Run

  `pip3 install flask`

  Flask will be installed as a global package.
3. Check if Flask is installed. Run

  `flask --version`

  You should see some version information printed.

  ```
  ❯ flask --version
  Python 3.10.9
  Flask 2.2.2
  Werkzeug 2.2.2
  ```

  If you don't, and get an error like "Command not found", then Flask is not
  installed!

## Run a Flask App

To start a flask application locally, navigate to a directory with a flask application and enter:

`flask run`

Try creating a minimal flask app and running it. In a new directory, create a file called `app.py` and add the following code to it:

```python
# app.py
from flask import Flask
app = Flask(__name__)

@app.get('/')
def index():
  return "Hello from Flask"
```

Save it, and enter `flask run` from that directory to start the application.

By default, flask will look for a file called `app.py`. If your app is named something else, you have to tell flask which file to run using the `--app` flag.

```sh
flask run --app server.py
```

## Installing in a virtual environment

As you are developing multiple applications on your computer, it's sometimes helpful to simulate different local environments with different packages installed. `virtualenv` is a tool for creating and managing virtual environments on one computer, so that each application only sees the packages that it is supposed to see.

1. To create a virtual environment, navigate to your project directory and run `python3 -m venv .`.
2. Then activate that environment with `source bin/activate`. You'll need to run this each time you switch to working on that project.
3. Install the dependencies (like flask) to that environment

> Remember: Each virtual environment has different packages installed! When you switch environments using `source bin/activate`, that 'turns on' a different set of installed packages. You need to install packages for each different virtual environment separately.

Some online resources are _adamant_ about using virtualenv. It's a good tool, but it has its own issues - mostly, you have to remember to juggle the virtual environment every time you switch projects. There's not just one way to install packages.

## Flask on Replit

Replit has a Flask template that handles the installation for you. You can create a new Repl with the Flask template, and then start coding right away. Replit also shows a preview of the pages of your site, and can connect to Github to have a repository of your code.

You can use Replit as an easy way to experiment with Flask, but we still require you to install Flask on your system locally to practice managing a local environment.

[Return to the README](./README.md)