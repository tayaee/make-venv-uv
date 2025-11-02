# Simple Python projects with requirements.txt
Use uv and requirements.txt to set up simple Python projects.

## Commands (Windows)
```
REM install-uv.bat
powershell -ExecutionPolicy Bypass -c "iwr https://astral.sh/uv/install.ps1 -useb | iex"
set "PATH=%USERPROFILE%\.local\bin;%PATH%"

REM make-venv-uv.bat
uv python pin 3.11
uv python install
uv venv .venv
call .venv\scripts\activate
uv pip compile requirements.txt -o uv.lock
uv pip sync uv.lock

python app.py
```

## Files
* Use `install-uv.bat` as Administrator to install uv.exe.
* Use `make-venv-uv.bat` to run all above commands.
* Use `make-venv-uv.bat 3.12` to switch Python version.
