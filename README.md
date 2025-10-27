Docker is a powerful tool for developing, packaging, and deploying applications efficiently. It uses containers, which can run consistently across different platforms. Docker is open-source and available for various operating systems, including Windows, macOS, and Linux. Dockers are faster compared to other software, like virtual machines, for running code across different platforms


FROM openjdk:24
# Pulls the OpenJDK 24 base image

RUN mkdir /app
# Creates a directory named 'app' inside the container

COPY out/production/Task-3/ /app
# Copies compiled Java files from the local directory to the container

WORKDIR /app
# Sets '/app' as the working directory

CMD java Main
# Runs the 'Main' class when the container starts

