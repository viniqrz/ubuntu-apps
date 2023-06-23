# Apps

## First run this to install homebrew

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

and this for bash config

obs: if you are using zsh, u gotta do additional work

```sh
test -d ~/.linuxbrew && eval "$(~/.linuxbrew/bin/brew shellenv)"
test -d /home/linuxbrew/.linuxbrew && eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
test -r ~/.bash_profile && echo "eval \"\$($(brew --prefix)/bin/brew shellenv)\"" >> ~/.bash_profile
echo "eval \"\$($(brew --prefix)/bin/brew shellenv)\"" >> ~/.profile
```


## VSCODE

this script has line breaks and will not run with simply copy & paste,
just paste it in browser address bar and copy

```sh
sudo snap install code --classic
```

## VLC PLAYER

```sh
sudo snap install vlc
```

## ZOOM

```sh
sudo snap install zoom-client
```

## NVM

```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

## SPOTIFY

```sh
sudo snap install spotify
```

## PYTHON

```sh
sudo apt install python3.9
```

## GIT

```sh
sudo apt install git
```

## DBEAVER-CE

```sh
sudo snap install dbeaver-ce
```

## CHROME

this script has line breaks and will not run with simply copy & paste,
just paste it in browser address bar and copy

```sh
sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list' &&
wget -q -O - https://dl.google.com/linux/linux_signing_key.pub | sudo apt-key add - &&
sudo apt-get update &&
sudo apt-get install google-chrome-stable
```

## DISCORD

```sh
sudo snap install discord
```

## INSOMNIA

```sh
sudo snap install insomnia
```

## ZSH

REMEMBER TO CONFIG BASH TERMINAL

```sh
sudo apt install zsh
```

## DOCKER

THIS IS TRICKY, IT WILL INSTALL, BUT YOU GOTTA DO ADDITIONAL CONFIG

```sh
sudo apt -y install docker.io
```

## DELUGE

```sh
sudo apt install deluge
```

## KUBECTL

```sh
sudo snap install kubectl --classic
```

## JDK

```sh
sudo apt-get install openjdk-11-jdk
```

## IDEA

```sh
sudo snap install intellij-idea-ultimate --classic
```

## FLUTTER

```sh
sudo snap install flutter --classic
```

## OH MY ZSH

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## RIPGREP

```sh
sudo apt-get install ripgrep
```

## MINIKUBE

```sh
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && sudo install minikube-linux-amd64 /usr/local/bin/minikube
```


# EVERYTHING TIED UP

```sh
sudo snap install code --classic && \
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" || \
  sudo apt-get install ripgrep || \
  sudo snap install flutter --classic && \
  sudo snap install kubectl --classic && \
  sudo apt -y install docker.io && \
  sudo apt -y install deluge && \
  sudo apt -y install zsh && \
  curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && \
  sudo install minikube-linux-amd64 /usr/local/bin/minikube && \
  sudo apt-get install openjdk-11-jdk && \
  sudo snap install insomnia && \
  sudo snap install discord && \
  sudo snap install dbeaver-ce && \
  sudo apt -y install git && \
  sudo snap install spotify && \
  sudo apt -y install python3 && \
  sudo snap install zoom-client && \
  sudo snap install vlc && \
  sudo snap install intellij-idea-ultimate --classic && \
  sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list' && \
  wget -q -O - https://dl.google.com/linux/linux_signing_key.pub | sudo apt-key add - && \
  sudo apt-get update && \
  sudo apt-get -y install google-chrome-stable && \
  sudo snap install android-studio --classic && \
  sudo snap install terraform --classic
```
