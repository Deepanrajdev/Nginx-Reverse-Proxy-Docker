# Use official Python slim image
FROM python:3.12-slim

# Set working directory
WORKDIR /app

# Install uv (a faster replacement for pip)
RUN pip install uv

# Copy project files
COPY . .

# Sync dependencies defined in pyproject.toml
RUN uv venv && uv sync

# Expose the Flask app port
EXPOSE 8002

# Run the Flask app using the created virtual environment
CMD [".venv/bin/python", "app.py"]

