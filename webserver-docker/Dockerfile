FROM ubuntu:18.04
RUN apt update; apt install -y gnupg2 

# Use an official Python runtime as the base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /flask_application

# Copy the requirements file into the container
COPY requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code
COPY . .

# Expose the port the app runs on
EXPOSE 8080

# Set environment variables (optional)
ENV FLASK_APP=run.py
# ENV FLASK_ENV=development

# Run the Flask application
CMD ["flask", "run", "--host=0.0.0.0"]

