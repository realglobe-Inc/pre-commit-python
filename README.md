# pre-commit-python
This repository is for Realglobe's shared pre-commit hooks.

## getting started
Run `pip install pre-commit` to install `pre-commit`. You can use `pipenv` as well.

Then create `.pre-commit-config.yaml` on your Python project's root.

```.pre-commit-config.yaml
repos:
  - repo: https://github.com/realglobe-Inc/pre-commit-python.git
    rev: '{commit hash or tag}'
    hooks:
      -   id: rg-hook
```

Run `pre-commit install --install-hooks` to install new pre-commit hook to `./git/hooks/`. If you use `pipenv`, run `pipenv run pre-commit install --install-hooks` instead. 
