FROM debian:bullseye-slim
ARG DEBIAN_FRONTEND=noninteractive 
RUN apt-get update && apt-get install -y curl gnupg && curl -sS https://apt.corretto.aws/corretto.key | gpg --dearmor > /etc/apt/trusted.gpg.d/corretto.gpg && echo "deb https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list && apt-get update && apt-get install -y java-17-amazon-corretto-jdk && apt-get autoremove -y curl gnupg && apt-get clean && rm -rf /var/lib/apt/lists/*
ENV PATH="$PATH:/usr/lib/jvm/java-17-amazon-corretto/bin"
