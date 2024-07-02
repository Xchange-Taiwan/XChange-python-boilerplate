# Python boilerplate

## Features
- ruff: linting and code formatting.
- pre-commit: pre-commit hooks.
- pytest: testing.
- logging: logging.
- devcontainer: vscode devcontainer.
- GitHub Actions: GitHub Actions.

## Usage

Change `python_template` folder name to your package name. Meanwhile, update the `name` in `pyproject.toml`.

### Use in local

#### (Strong Recommend) Install recommend VSCode extensions

I've listed the recommended vscode extensions in `.vscode/extensions.json`.<br>

Then, navigate to `Extensions` in VSCode. Install all extensions in `RECOMMENDED` tab.


#### Prepare development environment

##### Install poetry
```sh
curl -sSL https://install.python-poetry.org | python -
```

##### Use project default poetry
```sh
poetry sync
```

##### Install pre-commit hooks
```sh
poetry run pre-commit install
poetry run pre-commit install --hook-type commit-msg
```

### Use in dev container

#### Install dev container VSCode extension

Install `Dev Containers` extension in VSCode.

#### Open dev container

Click `ctrl + shift + p`, select `Dev Containers: Open Folder in Container`.<br>

Wait for the dev container to be built.

(if you want to left dev container running, click `ctrl + shift + p`, select `Dev Containers: Reopen Folder Locally`)
