# make-venv-uv
Use uv to manage dependencies in requirements.txt for simple Python projects.

## Related paths
* uv from PATH
* .python-version
* %APPDATA%\uv\python\
* .venv\
* requirements.txt
* uv.lock

As Administrator, install uv
```
install-uv.bat
```

## Three use cases
As regular user, install specific version of python, pin it at .python-version, create venv, create uv.lock from requirements.txt, install packages using uv.lock.
```
make-venv-uv.bat 3.12
```

As regular user, change python version (and in turn, re-create .venv and uv.lock)
```
make-venv-uv.bat 3.13
```

As regular user, install python configured in .python-version, create venv, create uv.lock from requirements.txt, install packages using uv.lock.
```
make-venv-uv.bat
```
