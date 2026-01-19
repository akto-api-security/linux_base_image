FROM amazonlinux:2023

# Install Corretto 8
RUN dnf install -y java-1.8.0-amazon-corretto \
    && dnf clean all

# Optional: verify
RUN java -version


WORKDIR /app
COPY ./target/mini-testing-1.0-SNAPSHOT-jar-with-dependencies.jar /app/mini-testing-1.0-SNAPSHOT-jar-with-dependencies.jar
CMD "java" "-XX:+ExitOnOutOfMemoryError" "-jar" "/app/mini-testing-1.0-SNAPSHOT-jar-with-dependencies.jar"

