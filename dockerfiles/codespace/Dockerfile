
# syntax=docker/dockerfile:1
FROM mcr.microsoft.com/devcontainers/python:3.12

# Install Jupyter + ipykernel + common scientific libs
RUN pip3 install --no-cache-dir --upgrade pip \
    && pip3 install --no-cache-dir jupyter jupyterlab ipykernel numpy matplotlib scipy imageio

# Optional: create workspace folder
RUN mkdir -p /workspaces

USER vscode
WORKDIR /workspaces

EXPOSE 8888
CMD ["sleep", "infinity"]
