# Use a small official devcontainer base image
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Install common tools (adjust as needed)
RUN apt-get update \
  && apt-get install -y --no-install-recommends \
    build-essential curl git python3 python3-pip nodejs npm \
  && apt-get clean && rm -rf /var/lib/apt/lists/*

# Optional: create a non-root user (devcontainers base already provides 'vscode')
USER vscode
