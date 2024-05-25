# Use the official Debian slim image from Docker Hub as a base
FROM python:3

# Set the working directory to /app
WORKDIR /usr/app

# Install Python3 and pip3
RUN apt-get update && apt-get install -y python3 python3-pip

# Copy the current directory contents into the container at /app
COPY . .

# Install Python packages
RUN pip3 install flask
RUN pip3 install pyjwt
RUN pip3 install pysqlite3

# Make port 8080 available to the world outside this container
EXPOSE 5000

# Run server.py when the container launches
CMD ["python3", "server.py"]