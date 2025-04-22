# oh-my-mac

## Homebrew

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```sh
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.bash_profile && source ~/.bash_profile
```

```sh
brew update && brew upgrade
```

```sh
# See https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/
git -C "$(brew --repo)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git
```

## Fonts

```sh
brew installfont-hack-nerd-font font-source-code-pro font-awesome-terminal-fonts font-fontawesome
```

https://github.com/tonsky/FiraCode

```sh
brew install --cask font-fira-code font-fira-mono font-fira-mono-for-powerline font-fira-sans
```

```sh
brew install --cask powerline-fonts
```

## Zsh

```sh
brew install zsh zsh-completions
```

```sh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

```sh
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.zshrc && source ~/.zshrc
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.bash_profile && source ~/.bash_profile
```

## 图形界面

Development

```sh
brew install --cask iterm2
brew install --cask alfred
brew install --cask dash
brew install --cask charles
brew install --cask wireshark
brew install --cask switchhosts
brew install --cask paw
brew install --cask tower
brew install --cask vagrant-manager
brew install --cask virtualbox
```

Tools

```sh
brew install --cask istat-menus
brew install --cask paste
brew install --cask spectacle
brew install --cask shadowsocks-ng
brew install --cask scroll-reverser
brew install --cask background-music
```

```sh
brew install --cask iina
brew install --cask neteasemusic
brew install --cask itsycal
brew install --cask qq
brew install --cask wechat
brew install --cask wechatwebdevtools
brew install --cask dingtalk
brew install --cask telegram
brew install --cask sketch
brew install --cask ithoughtsx
brew install --cask eudic
brew install --cask cheatsheet
brew install --cask scroll-reverser
```

```sh
brew install --cask eagle
brew install --cask feedly
brew install --cask notion
brew install --cask marginnote
brew install --cask tingings
brew install --cask timing
brew install --cask xmind-zen
brew install --cask pantastical
brew install raindrop.io
```

```sh
brew cask install 1password
brew cask install steermouse
brew cask install neteasymusic
brew cask install keka
brew cask install handshaker
brew cask install firefox
brew cask install neteasemusic
brew cask install firefox
brew cask install qqlive
brew cask install qqmusic
brew cask install phpstorm
brew cask install corkscrem
brew cask install phpdocumentor
brew cask install keycastr
brew cask install omnifocus
brew cask install omnioutliner
brew cask install omnigraffle
brew cask install omniplan
brew cask install mindnode-pro
brew cask install steam
brew cask install sketch
brew cask install evernote
brew cask install hyperdock
brew cask install hyperswitch
brew cask install sogouinput
brew cask install gas-mask
brew cask install adobe-acrobat-reader
brew cask install slack
brew cask install discord
brew cask install gitter
brew cask install trello
brew cask install raindropio
brew cask install clion
```

```sh
brew install --cask microsoft-office
```

## 命令行

Shell

```sh
brew install antigen asciinema mosh tmux elvish hyper
```

```sh
brew install vitorgalvao/tiny-scripts/cask-repair
brew install automake autoconf curl pcre bison re2c mhash icu4c gettext jpeg openssl mcrypt gmp BZip2 iconv
brew install libtool libxml2 libevent zlib libiconv
```

```sh
brew install mas
```

Jump

```sh
brew install z autojump thefuck
```

Editor

```sh
brew install vim bvi neovim
brew install --cask emacs
```

Git

```sh
brew install git git-flow git-extras pre-commit tig
brew install --cask gitup
```

Build Tools

```sh
brew install gcc gdb make cmake ctags pkg-config
brew install cairo pango libpng jpeg giflib
```

Common Commands

```sh
brew install openssl cfssl easy-rsa
brew install coreutils gnutls gnupg
brew install htop nload
brew install pstree
brew install wget curl telnet
brew install exa tree
brew install unzip xz
brew install iproute2mac
brew install ack fasd ag fzf
brew install md5sha1sum
brew install mycli
brew install jq
brew install ncdu
```

```sh
brew install lrzsz
# https://github.com/aurora/iterm2-zmodem
```

Development

```sh
brew install node nvm yarn
brew install python python3 pyenv-virtualenv pyenv virtualenv pip pipenv
brew install ruby rbenv
brew install go goenv dep go-delve/delve/delve
brew install php
brew install rust
brew install r
brew install perl
brew install qt
brew install java
brew install ipython
brew install dart
brew install rustup
brew install flutter
brew install jupyter
brew install chromedriver
brew install qemu
```

```sh
brew install phpbrew
brew install phpenv
brew install php-version
brew install phpdocumentor
brew install phpdoc
brew install xdebug
brew install brew-php-switcher php-code-sniffer php-cs-fixer phplint phpstan phpunit
```

```sh
brew tap hhvm/hhvm
brew install hhvm
```

```sh
brew install cloc
brew install bazel
```

```sh
brew install travis
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

Proxy

```sh
brew install openvpn
brew install shadowsocks-libev
brew install proxychains-ng
brew install privoxy
brew install tsocks
brew install mitmproxy
brew install --cask v2rayx
brew install --cask v2rayu
```

```sh
brew cask install ngrok
```

```sh
brew install corkscrew
brew install connect
```

Docker & k8s

```sh
brew install docker
brew install kubectl
brew upgrade kubernetes-cli
brew install kubernetes-helm
brew install helm
```

```sh
brew install --cask docker
brew install --cask minikube
```

```sh
brew install etcd
```

## Skill

命令行支持 TouchID

```sh
➜ cat /etc/pam.d/sudo
# sudo: auth account password session
auth       sufficient     pam_smartcard.so
auth       required       pam_opendirectory.so
account    required       pam_permit.so
password   required       pam_deny.so
session    required       pam_permit.so
```

```sh
sudo sed -i ".bak" '2s/^/auth       sufficient     pam_tid.so\'$'\n/g' /etc/pam.d/sudo
```

```sh
➜ cat /etc/pam.d/sudo
# sudo: auth account password session
auth       sufficient     pam_tid.so
auth       sufficient     pam_smartcard.so
auth       required       pam_opendirectory.so
account    required       pam_permit.so
password   required       pam_deny.so
session    required       pam_permit.so
```

backupfile: /etc/pam.d/sudo.bak

* [iTerm does not opening Touch ID auth dialog anymore](https://gitlab.com/gnachman/iterm2/issues/7608)

## Q&A

* [LC_CTYPE: cannot change locale](https://www.jianshu.com/p/2b24861be987)
