FROM maven:3.9-eclipse-temurin-11-alpine

# Install bash, git, and Docker CLI tools
RUN apk add --no-cache \
    bash \
    git \
    docker-cli \
    docker-cli-buildx

# Verify all required tools are installed
RUN java -version && \
    mvn -version && \
    git --version && \
    docker --version && \
    bash --version

WORKDIR /app
