FROM ubuntu:latest

# Install core requirements for oh-my-zsh
RUN apt-get update \
    && apt-get -y install git-core \
                          curl \
                          zsh \

# Install oh-my-zsh
RUN sh -c "$(curl -fsSL https://raw.githubusercontent.com/hnt4499/oh-my-zsh/master/tools/install.sh)"

# Install and generate locales as well as fonts for "agnoster" theme.
RUN apt-get -y install locales \
                       fonts-powerline \
    && locale-gen en_US.UTF-8 \
    && source ~/.zshrc

CMD ["zsh"]

