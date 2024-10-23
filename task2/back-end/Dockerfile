# Latest version of Ubuntu.
FROM ubuntu:latest
# Update APT.
RUN apt-get update
# Upgrade currently installed software.
RUN apt-get upgrade -y
# Run command in terminal.
CMD ["echo", "Hello, World!"]
# Install python3.
RUN apt-get install -y python3
# Install python3-pip.
RUN apt-get install -y python3-pip
# Install flask (Externally Managed).
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install Flask
# Use "app" as the working directory.
WORKDIR /app
# Copy the Python file to Docker image.
COPY api.py /app
# Host Flask app on port 5252
EXPOSE 5252