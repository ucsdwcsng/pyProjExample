# Python Project Example

This is meant to be a boilerplate repo that shows you how to setup a
python project that uses developer tools such as

1. pre-commit - when you run `git commit` a set of user defined tests will
automatically be run on your code before the commit is allowed to complete. If
any of the tests fail, the commit will fail and you will need to fix the errors
and try again. This prevents bad commits from making it into the repo. https://pre-commit.com/
2. poetry - this is a dependency management tool that keeps track of all the
required modules needed to run your project. When you want to use your project
on another computer, or update the modules you are using, poetry makes this
easy and automatic. https://python-poetry.org/docs/
3. github actions - this allows you to automatically run tests on code that are
commited to the remote repo. It can be activated by various events like pull
requests. An example use case is when a pull request is made on the main
branch, a set of actions can be triggered and the code must pass for the pull
request to be completed. https://docs.github.com/en/actions
4. virtualenv - this is one of the popular virtual environment managers. https://realpython.com/python-virtual-environments-a-primer/#the-virtualenv-project
5. pytest - this is a unit testing module that makes testing python code easy. https://realpython.com/pytest-python-testing/
6. cmd module - this is a module that makes creation of command line interfaces
in python easy. https://docs.python.org/3/library/cmd.html
7. logging module - this is a module that makes logging easy. https://betterstack.com/community/guides/logging/how-to-start-logging-with-python/
8. pytorch module - the ubiquotous machine learning module for python. The
cuda version will be installed allowing you to train machine learning algorithms
using a GPU. If you do not have a supported GPU, this may fail to install. https://pytorch.org/

## How to use this project

1. Make sure poetry is installed. 
Follow the instructions for installing poetry using the script method. 
I recommend you do not use `pipx` or `pip` to install poetry as the version 
you get tends to be older. This project was made with poetry v1.3.2.\
`curl -sSL https://install.python-poetry.org | python3 -`
2. `git clone git@github.com:rcbell1/pyProjExample.git`
3. `cd pyProjExample`
4. `mdkir ~/virtualenvs && virtualenv ~/virtualenvs/pyexamp`
5. `source ~/virtualenvs/pyexamp/bin/activate`
6. `poetry install`
7. `pre-commit install`
