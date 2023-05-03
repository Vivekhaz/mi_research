# Getting Setup with our Dev ENV

This is ideally very temporary.

## STEP 1: Python Stuff

### 1.A
Make sure you have homebrew installed
```
```

### 1.B
Then: install pyenv, 
```
brew install pyenv
echo 'eval "$(pyenv init --path)"' >> ~/.zshrc
pyenv install 3.10.5
```

### 1.C
Then: install poetry, a python package manager.
```
curl -sSL https://install.python-poetry.org | python3 -
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zprofile
```


## STEP 2: Our Library Stuff

We have a dev container that you can open in VSCode and it should auto 
install all the right packages and recommended extensions.

```
poetry config virtualenvs.in-project true
poetry install --with dev
```
