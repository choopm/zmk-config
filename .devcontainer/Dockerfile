FROM zmkfirmware/zmk-dev-arm:3.5

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get install -y \
    curl \
    sudo \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/* \
    && echo 'ubuntu ALL=(ALL:ALL) NOPASSWD: ALL' > /etc/sudoers.d/01_ubuntu

# install go-task
RUN curl -sSL https://github.com/go-task/task/releases/latest/download/task_linux_amd64.deb -o /tmp/task.deb && \
    dpkg -i /tmp/task.deb && \
    rm /tmp/task.deb

LABEL org.opencontainers.image.source=https://github.com/choopm/zmk-config
