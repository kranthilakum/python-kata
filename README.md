
### Virtual Environment

The `venv` module creates a lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. 

A virtual environment is created on top of an existing Python installation, known as the virtual environment’s “base” Python, and may optionally be isolated from the packages in the base environment, so only those explicitly installed in the virtual environment are available.

Creation of virtual environments is done by executing the command venv:

```bash
python3 -m venv /path/to/new/virtual/environment/venv
# Activate virtual environment
.\venv\Scripts\activate.bat
# Deactivate virtual environment
deactivate
# install packages
pip install pip-tools
# create requirements.in and add packages

# compile requirements.in and auto-generate requirements.txt
pip-compile --output-file=- > requirements.txt

# If you have to update a dependency you just need to update the requirements.in file and redo pip-compile
```

Alternatively, you can use `virtualenv`, a third party application (and predecessor to venv). It allows virtual environments to be used on versions of Python prior to 3.4, which either don’t provide venv at all, or aren’t able to automatically install pip into created environments.

To create a virtual environment using `virtualenv`, run the following command:

```bash
    virtualenv venv
```

#### Links
- [venv - Creation of virtual environments](https://docs.python.org/3/library/venv.html)
- [Creating a virtual enviornment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)

Licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)

[Google's Python Class](http://code.google.com/edu/languages/google-python-class/)

