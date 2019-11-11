# oh-my-mac

## Homebrew

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
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
brew cask install font-hack-nerd-font
brew cask install font-source-code-pro
brew cask install font-awesome-terminal-fonts
brew cask install font-fontawesome
```

https://github.com/tonsky/FiraCode

```sh
brew cask install font-fira-code font-fira-mono font-fira-mono-for-powerline font-fira-sans
```

```sh
brew cask install powerline-fonts
```

## Zsh

```sh
brew install zsh zsh-completions
```

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

```sh
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.zshrc && source ~/.zshrc
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.bash_profile && source ~/.bash_profile
```

## 图形界面

Development

```sh
brew cask install iterm2
brew cask install alfred
brew cask install dash
brew cask install charles
brew cask install wireshark
brew cask install switchhosts
brew cask install paw
brew cask install tower
brew cask install vagrant-manager
brew cask install virtualbox
```

Tools

```sh
brew cask install istat-menus
brew cask install paste
brew cask install spectacle
brew cask install shadowsocks-ng
brew cask install scroll-reverser
brew cask install background-music
```

```sh
brew cask install iina
brew cask install neteasemusic
brew cask install itsycal
brew cask install qq
brew cask install wechat
brew cask install wechatwebdevtools
brew cask install dingtalk
brew cask install telegram
brew cask install sketch
brew cask install ithoughtsx
brew cask install eudic
brew cask install cheatsheet
brew cask install scroll-reverser
```

```sh
brew cask install eagle
brew cask install feedly
brew cask install notion
brew cask install marginnote
brew cask install tingings
brew cask install timing
brew cask install xmind-zen
brew cask install pantastical
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
brew cask install trello
brew cask install raindropio
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
brew cask install v2rayx
brew cask install v2rayu
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
brew cask install docker
brew cask install minikube
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
