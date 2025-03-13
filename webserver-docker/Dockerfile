FROM ubuntu:18.04
RUN apt update; apt install -y gnupg2

RUN apt install python3-pip

# Use an official Python runtime as the base image
FROM python:3.8

# Set the working directory in the container
WORKDIR /flask_application

# Copy the requirements file into the container
COPY . /flask_application

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port the app runs on
EXPOSE 8080

# Set environment variables (optional)
# ENV FLASK_APP=run.py
# ENV FLASK_ENV=development

# Run the Flask application
CMD ["python", "run.py", "--host=0.0.0.0"]

