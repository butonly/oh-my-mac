# oh-my-mac

## 必备软件

* iTerm2
* Alfred
* SwitchHosts
* Paw
* Charles
* Dash

* iStats
* Paste
* Spectacle
* Scroll Reverser
* ShadowSocks

## Homebrew

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

```sh
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.zshrc
source ~/.zshrc
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.bash_profile
source ~/.bash_profile
```

```sh
# See https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/
cd "$(brew --repo)"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-science"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-science.git
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-python"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-python.git
```

```sh
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall)"
curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall
```

```sh
brew tap homebrew/cask
brew tap homebrew/science
brew tap homebrew/fonts
```

```sh
brew update && brew upgrade
```

## 命令行

Shell

```sh
brew install zsh antigen mosh tmux powerline elvish hyper
```

Productivity

```sh
brew install z autojump thefuck asciinema
```

Editor

```sh
brew install vim bvi neovim emacs
```

Git

```sh
brew install git git-flow git-extras git-flow-avh pre-commit tig
```

Build Tools

```sh
brew install gcc gdb make build-essential cmake ctags pkg-config
brew install cairo pango libpng jpeg giflib
```

```sh
brew install node nvm npx yarn
brew install python python3 pyenv-virtualenv pyenv virtualenv pip pipenv
brew install ruby rbenv
brew install go goenv dep go-delve/delve/delve
brew install php php5 php56 phpbrew
brew install rust
brew install r
brew install perl
brew install qt
brew install chromedriver
```

```sh
brew install cloc
brew install bazel
```

Server Service Software

```sh
brew install mongodb redis mysql postgresql etcd consul
brew install elasticsearch logstash kinaba filebeat
brew install prometheus grafana influxdb collectd
brew install graphicsmagick graphviz
brew install dnsmasq nginx httpd vegeta
brew install ansible
brew install vagrant
brew install jenkins
```

Common Commands

```sh
brew install openssl cfssl easyrsa
brew install coreutils gnupg gnutls
brew install htop nload
brew install pstree
brew install wget curl telnet
brew install exa tree
brew install unrar xz
brew install ip iproute2mac
brew install ack fasd ag fzf
brew install md5sum
brew install gcloud
brew install mycli
```

Proxy

```sh
brew install openvpn
brew install shadowsocks-libev
brew install proxychains-ng
brew install privoxy
brew install tsocks
brew install mitmproxy
brew cask install ngrok
```

Docker & k8s

```sh
brew install docker
brew install kubectl
brew upgrade kubernetes-cli
brew install kubernetes-helm
brew install helm
brew cask install minikube
```

Fonts

```sh
brew cask install font-hack-nerd-font
brew cask install font-source-code-pro
brew cask install font-awesome-terminal-fonts
brew cask install font-fontawesome
```

iTerm2 Extensions

```sh
brew install sudolikeaboss
```
