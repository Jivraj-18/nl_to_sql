FROM python:3.12-slim-bookworm

# Use uv from ghcr
COPY --from=ghcr.io/astral-sh/uv:latest /uv /uvx /bin/

WORKDIR /app

COPY . .


# Default command
CMD ["sh", "-c", "uv run json_to_database.py && uv run main.py"]
