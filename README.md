# Scientific Computing Toolbox

![Tests](https://github.com/R3sten/SCToolbox/actions/workflows/tests.yml/badge.svg)

This project aims to be both an homework for the Advanced Programmin class that I have just took and a way to learn how to build a well structured Python/C++ project with well implemented tests and continuous integration workflow.

## Do you want to build this project?

First you have to clone this repositry in your desired location:

```
git clone https://github.com/R3sten/SCToolbox.git
```

Then I highly recommend to create a virtual environment and activate it:

```
$ python -m venv venv

$ source venv/bin/activate
```

Then install the packages needed to run the software and build the local library:

```
$ pip install -r requirements.txt

$ pip install .
```

If you want to modify the code you can also install the local libray in editable mode:

```
$ pip install -e .
```

## Testing:

First, in order to run tests, you have to install the dependencies related to them:

```
$ pip install -r requirements_dev.txt
```

### Type checking:

For testing the code structure and correctnes you can run the folowing commands:

```
$ mypy src

$ flake8 src tests
```

### Software functionality tests:

For testing the code into current enviroment you can simply run from the root of the project:

```
$ pytest
```

Also you can test it into different Python environments.
If not already installed, Python interpreters that that are going to be used during the tests need to be downloaded before:

```
$ sudo apt update
$ sudo apt install software-properties-common
$ sudo add-apt-repository ppa:deadsnakes/ppa

$ sudo apt install python3.10 python3.11 python3.12 python3.13
```

Then simply you have just to run tox and automatically tests are being done:

```
tox
```
