FROM ubuntu:latest

# Set the working directory in the image
WORKDIR /app

# Copy the files from the host file system to the image file system
COPY . /app

# Install the necessary packages
RUN apt-get update && apt-get install -y python3 python3-pip

# Debug: List contents of /app
RUN ls -la /app

# Debug: List contents of /app/examples/first-docker-file
RUN ls -la /app/doss/examples/first-docker-file

# Set environment variables
ENV NAME World

# Set the correct working directory if the app.py is in a nested directory
WORKDIR /app/doss/examples/first-docker-file

# Run a command to start the application
CMD ["python3", "app.py"]
