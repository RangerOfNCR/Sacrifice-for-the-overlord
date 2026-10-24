.PHONY: lint format format-check typecheck check fix precommit

lint:
	ruff check .

format:
	ruff format .

format-check:
	ruff format --check .

typecheck:
	pyright

fix:
	ruff check . --fix

check: lint format-check typecheck

precommit:
	pre-commit install --hook-type pre-commit --hook-type pre-push