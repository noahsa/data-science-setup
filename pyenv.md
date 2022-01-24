# Pyenv

Pyenv can be intimidating. I started using Pyenv when Poetry started giving me errors while creating virtual environments.

## Activate virtual environment with Poetry

Poetry is giving me errors when it tries to create the virtual environment. Instead, I'll use pyenv to create the virtual environment. Poetry still figures out which dependencies work together. I just convert the poetry specification to `requirements.txt`. Then, install into a pyenv created virtual environment.

```bash
poetry export -f requirements.txt --output requirements.txt --without-hashes --dev
python -m venv venv
source venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```
