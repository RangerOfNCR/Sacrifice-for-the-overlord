.PHONY: lint format format-check typecheck check fix

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
