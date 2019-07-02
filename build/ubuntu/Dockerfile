FROM ubuntu:latest

# Install core requirements for zsh
RUN apt-get update \
    && apt-get -y install git \
                          curl \
                          zsh \
                          fonts-powerline

# Install and generate locales
RUN apt-get -y install locales \ 
    && locale-gen en_US.UTF-8

# Install oh-my-zsh
RUN sh -c "$(curl -fsSL https://raw.githubusercontent.com/hnt4499/oh-my-zsh/master/tools/install.sh)"

CMD ["zsh"]

