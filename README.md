# research-template

Minimalistic template for research in Python. Linters, code format, PEP8.

## Requirements

- Install pre-commit
  ```bash
  pip install -U pip
  pip install pre-commit
  ```
- Install the hooks, run this command inside the folder
  ```bash
  pre-commit install
  ```

## Git Workflow

- `development` branch is where all up-to-date stable code is maintained
- `feature/feature-name` is a branch for any improvement, bugs, refactoring or documentation. This branch is the one used to push changes to `development` through Pull Request (PR)

## To create a pull request:

1. Clone the repository
2. Install pre-commit hook:

```bash
    pip install pre-commit black flake8 isort
```

3. Initialize it from the folder within the repo:

```bash

    pre-commit install
```

4. Create `feature/feature-name` branch

5. Make desired changes to the code

6. Run `pre-commit run --all-files` and fix errors

7. Push code to your `feature/feature-name` branch

8. Create pull request
