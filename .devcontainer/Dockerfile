ARG VARIANT=3-bullseye
FROM mcr.microsoft.com/vscode/devcontainers/python:${VARIANT}

USER vscode
RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python -

ARG USERNAME=vscode

RUN mkdir -p /home/$USERNAME/.vscode-server/extensions \
    && chown -R $USERNAME \
    /home/$USERNAME/.vscode-server \
