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
brew install font-hack-nerd-font font-source-code-pro font-awesome-terminal-fonts font-fontawesome
```

https://github.com/tonsky/FiraCode

```sh
brew install font-fira-code font-fira-mono font-fira-mono-for-powerline font-fira-sans
```

```sh
brew install powerline-fonts
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
brew install iterm2
brew install alfred
brew install dash
brew install charles
brew install wireshark
brew install switchhosts
brew install paw
brew install tower
brew install vagrant-manager
brew install virtualbox
```

Tools

```sh
brew install istat-menus
brew install paste
brew install spectacle
brew install shadowsocks-ng
brew install scroll-reverser
brew install background-music
```

```sh
brew install iina
brew install neteasemusic
brew install itsycal
brew install qq
brew install wechat
brew install wechatwebdevtools
brew install dingtalk
brew install telegram
brew install sketch
brew install ithoughtsx
brew install eudic
brew install cheatsheet
brew install scroll-reverser
```

```sh
brew install eagle
brew install feedly
brew install notion
brew install marginnote
brew install tingings
brew install timing
brew install xmind-zen
brew install pantastical
brew install raindrop.io
```

```sh
brew install 1password
brew install steermouse
brew install neteasymusic
brew install keka
brew install handshaker
brew install firefox
brew install neteasemusic
brew install firefox
brew install qqlive
brew install qqmusic
brew install phpstorm
brew install corkscrem
brew install phpdocumentor
brew install keycastr
brew install omnifocus
brew install omnioutliner
brew install omnigraffle
brew install omniplan
brew install mindnode-pro
brew install steam
brew install sketch
brew install evernote
brew install hyperdock
brew install hyperswitch
brew install sogouinput
brew install gas-mask
brew install adobe-acrobat-reader
brew install slack
brew install discord
brew install gitter
brew install trello
brew install raindropio
brew install clion
```

```sh
brew install microsoft-office
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
brew install emacs
```

Git

```sh
brew install git git-flow git-extras pre-commit tig
brew install gitup
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
brew install v2rayx
brew install v2rayu
```

```sh
brew install ngrok
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
brew install docker
brew install minikube
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
