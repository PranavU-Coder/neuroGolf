# Guidelines

Hi, now do as I say

## Dependency Manager

if you still use pip in 2026, please fuck off.

please use [uv](https://docs.astral.sh/uv/getting-started/installation/#standalone-installer)

once installed in your system, please run this command:

```bash
uv sync
```

this will pick up all the dependencies from the lock file as was in the original project.

Strictly adhering to PEP-8 convention, ruff will be used for linting and code formatting.

```bash
 uv run ruff format .
 ```

## Tests

Right now there are no real tests, till actual work will be done however it is necessary to pass **ALL THE TESTS** else PR is rejected by default.

before creating a new PR, please run this command:

```bash
python -m pytest
```

## Docstring Coverage

Please document your functions/classes aptly, keep it brief.
Explain all parameters being inputted in a function and the expected output.

ALSO FOR THE LOVE OF GOD, make sure most if not all variables have **STATIC TYPE ANNOTATION**. These are good programming practicecs which should be adhered to.

## Report Issues

[WIP]

## Versioning

Commit only if it is needed, with each feat/fix/chore etc, version in `pyproject.toml` must be bumped accordingly.

## Commit Prefixes

Please include `fix` `feat` `chore` `migration` `docs` etc in accordance to your action, not doing so will have your PR rejected as well.

Please see `git log --oneline` to understand this.
