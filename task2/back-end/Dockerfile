# Base image
FROM ubuntu:latest

# Update & upgrade
RUN apt-get update
RUN apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Fix "externally managed" pip error (Ubuntu 23+ üçün)
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set working directory
WORKDIR /app

# Copy Flask app
COPY api.py /app/api.py

# Run Flask app
CMD ["python3", "/app/api.py"]
