Docker is a powerful tool for developing, packaging, and deploying applications efficiently. It uses containers, which can run consistently across different platforms. Docker is open-source and available for various operating systems, including Windows, macOS, and Linux. Dockers are faster compared to other software, like virtual machines, for running code across different platforms


FROM openjdk:24    (pulls from the version of JDK being worked on)
RUN mkdir / app     (makes a directory called app)
COPY out/production/Task-3/ /app      (copies from files to run) 
WORKDIR /app             (Either puts it into App or runs it in app)
CMD java Main             (Runs the "main" file)
