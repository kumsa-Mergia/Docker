```DOCKERFILE
FROM python:3.9-slim-buster

# Set the working directory
WORKDIR /app

# Copy the requirements file
COPY requirements.txt requirements.txt

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application code
COPY . .

# Expose the port
EXPOSE 8000

# Define environment variables (optional)
ENV MY_ENV_VAR="some_value"

# Start the application
CMD ["gunicorn", "--bind", "0.0.0.0:8000", "my_app:app"]

```
