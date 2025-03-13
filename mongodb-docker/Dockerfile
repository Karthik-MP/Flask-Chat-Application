FROM ubuntu:18.04
RUN apt update; apt install -y gnupg2 

# Use the official MongoDB image
FROM mongo:latest

# Set environment variables (optional)
# ENV MONGO_INITDB_ROOT_USERNAME=admin
# ENV MONGO_INITDB_ROOT_PASSWORD=password

# Expose the MongoDB port
EXPOSE 27017

# Start MongoDB with custom bindIp setting
CMD ["mongod", "--bind_ip", "0.0.0.0"]