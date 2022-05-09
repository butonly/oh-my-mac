# oh-my-mac

## Homebrew

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```sh
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.bash_profile && source ~/.bash_profile
```

```sh
brew tap homebrew/cask
brew tap homebrew/cask-fonts
brew tap homebrew/cask-versions
```

```sh
brew update && brew upgrade
```

```sh
# See https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/
git -C "$(brew --repo)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git
git -C "$(brew --repo)/Library/Taps/homebrew/homebrew-core" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git
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
brew install --cask 1password
brew install --cask steermouse
brew install --cask neteasymusic
brew install --cask keka
brew install --cask handshaker
brew install --cask firefox
brew install --cask neteasemusic
brew install --cask firefox
brew install --cask qqlive
brew install --cask qqmusic
brew install --cask phpstorm
brew install --cask corkscrem
brew install --cask phpdocumentor
brew install --cask keycastr
brew install --cask omnifocus
brew install --cask omnioutliner
brew install --cask omnigraffle
brew install --cask omniplan
brew install --cask mindnode-pro
brew install --cask steam
brew install --cask sketch
brew install --cask evernote
brew install --cask hyperdock
brew install --cask hyperswitch
brew install --cask sogouinput
brew install --cask gas-mask
brew install --cask adobe-acrobat-reader
brew install --cask slack
brew install --cask discord
brew install --cask trello
brew install --cask raindropio
```

## 命令行

Shell

```sh
brew install antigen asciinema mosh tmux powerline elvish hyper
```

```sh
brew install vitorgalvao/tiny-scripts/cask-repair
brew install automake autoconf curl pcre bison re2c mhash libtool icu4c gettext jpeg openssl libxml2 mcrypt gmp libevent zlib BZip2 libbz2-dev iconv libiconv
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
brew install vim bvi neovim emacs
```

Git

```sh
brew install git git-flow git-extras git-flow-avh pre-commit tig gitup
```

Build Tools

```sh
brew install gcc gdb make build-essential cmake ctags pkg-config
brew install cairo pango libpng jpeg giflib
```

Common Commands

```sh
brew install openssl cfssl easyrsa
brew install coreutils gnutls gnupg
brew install htop nload
brew install pstree
brew install wget curl telnet
brew install exa tree
brew install unrar unzip xz
brew install ip iproute2mac
brew install ack fasd ag fzf
brew install md5sum
brew install gcloud
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
brew install node nvm npx yarn
brew install python python3 pyenv-virtualenv pyenv virtualenv pip pipenv
brew install ruby rbenv
brew install go goenv dep go-delve/delve/delve
brew install php php5 php56 phpbrew
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
brew install hhvm
brew install xdebug
brew install brew-php-switcher php-code-sniffer php-cs-fixer phplint phpstan phpunit 
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
