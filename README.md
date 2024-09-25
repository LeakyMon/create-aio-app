# Create Aio App

[![Build Status](https://travis-ci.com/aio-libs/create-aio-app.svg?branch=master)](https://travis-ci.com/aio-libs/create-aio-app)  
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)  
[![Gitter chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/aio-libs/Lobby)  
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-green.svg)](https://github.com/aio-libs/create-aio-app/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)  
[![PyPI version](https://badge.fury.io/py/create-aio-app.svg)](https://badge.fury.io/py/create-aio-app)

The tool that lets you bootstrap aiohttp applications with best practices ready for development.

## Screenshot of Interface
![Example](https://raw.githubusercontent.com/aio-libs/create-aio-app/master/assets/assets.png)

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Salient Features](#salient-features)
4. [Options](#options)
5. [Troubleshooting](#troubleshooting)
6. [Contributing](#contributing)
7. [License](#license)

## Installation

### Requirements

- Python 3.6+
- Docker (optional, for deployment)
- Docker Compose

### Verify Installation
To ensure Python and Docker are installed, run:
    ```bash
    python --version
    docker --version
    ```

### Install Python

Ensure Python 3.6 or higher is installed:

- **Windows**: Download Python from [here](https://www.python.org/downloads/) and check "Add Python to PATH" during installation.
- **macOS**: Install Python using Homebrew:
  ```bash
  brew install python

- **Linux**: Use your package manager to install Python
    ```bash
    sudo apt-get update
    sudo apt-get install python3
    ```


## Usage

```bash
create-aio-app my_project
```

If you want to use interactive mode enter the next command:

```bash
create-aio-app
```

This will create a new directory called `my_project`.
To start you new project run the next commands:

```bash
cd my_project

make run # start your project
```

[Here is a link to all the make commands.](https://create-aio-app.readthedocs.io/pages/commands.html)

## Real-World Example Use Case

An example case for this program is to setup a basic API server in aiohttp responsible for handling async web requests.
The setup will include all the necesities to start your async API efficiently with the best built in practices.

Now, navigate in your browser to `http://localhost:8080/`

## Salient Features

- [aiohttp](https://aiohttp.readthedocs.io/en/stable/) - the best python framework :)
- [mypy](https://mypy.readthedocs.io/en/latest/) - optional static typing
- [pytest](https://pytest.readthedocs.io/en/latest/) - unit tests
- [flake8](https://flake8.readthedocs.io/en/latest/) - linter
- [black](https://black.readthedocs.io/en/latest/) - code formatter
- [trafaret](https://trafaret.readthedocs.io/en/latest/) - data validation
- [aio devtools](https://github.com/aio-libs/aiohttp-devtools) - developer tools
- [aiohttp debug toolbar](https://github.com/aio-libs/aiohttp-debugtoolbar) - tool for debugging
- [postgres](https://www.postgresql.org/) - storage
- [alembic](https://alembic.sqlalchemy.org/en/latest/tutorial.html) - database migration tool
- [sqlAlchemy](https://www.sqlalchemy.org/) - orm
- [sphinx](http://www.sphinx-doc.org/en/master/) - docs
- [docker-compose](https://docs.docker.com/compose/) - tool for defining and running multi-container Docker applications
- [py-spy](https://github.com/benfred/py-spy) - Sampling profiler for Python programs

## Options

`--without-postgres` - remove postgres and all of its requirements

`--redis` - add redis to the template

`--uvloop` - uvloop event loop for aiohttp

## Troubleshooting
Common Issues

- Issue: "ModuleNotFoundError: No module named 'aiohttp'"
    - You must ensure that you have activated the virtual environment (venv) and installed ALL the required dependencies. If the problem continues, opt to run the following
    ```bash 
    source venv/bin/activate 
    pip install -r requirements.txt
    ```

- Docker Error: "Permission Denied"
    - Ensure Docker is running and that you have the correct permissions. On Linux, add your user to the Docker group:
    ```bash 
    sudo usermod -aG docker $USER
    ```
    - MUST RESTART TERMINAL BEFORE TRYING AGAIN!

## Contributing

`create-aio-app` is a boilerplate from aiohttp community for aiohttp 
community. Feel free to make any suggestions on the issues or 
create a pull request. We will be very happy 😀. 
See [CONTRIBUTING.md](https://github.com/aio-libs/create-aio-app/blob/master/CONTRIBUTING.md) for more information about 
how to contribute to `create-aio-app`.

## License

Create aio App is an open source software <a href="https://github.com/aio-libs/create-aio-app/blob/master/LICENSE">available under the MIT license</a>.
