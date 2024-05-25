# Use the official Dart image from Docker Hub as a base
FROM dart:latest

# Set the working directory to /app
WORKDIR /usr/app

# Copy the current directory contents into the container at /app
COPY . .

# Get dependencies for the Dart project
RUN dart pub get

# Make port 80 available to the world outside this container
EXPOSE 80

# Run the Dart application when the container launches
CMD ["dart", "run", "/usr/app/bin/social_wall.dart"]