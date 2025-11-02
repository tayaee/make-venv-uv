# Simple Python project wiht requirements.txt
Use uv and requirements.txt to set up simple Python projects.

## Set up
Use `install-uv.bat` as Administrator to install uv.exe.

## Use
Use `make-venv-uv.bat 3.11` to install Python 3.11 (or 3.12, 3.13, 3.14), pin the python version at .python-version, create .venv, activate .venv, create uv.lock from requirements.txt, install packages using uv.lock.

Use `make-venv-uv.bat 3.12` (or other versions) to switch Python version.

Use `make-venv-uv.bat` to install Python configured in .python-version, create .venv, activate .venv, create uv.lock from requirements.txt, install packages using uv.lock.
