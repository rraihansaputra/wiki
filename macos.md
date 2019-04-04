# MacOS reSetup Guideline

## resources for setting up
**[dotfiles.github.io](https://dotfiles.github.io/)**  
**[dotfiles using dotbot and vscode and stuff](https://github.com/sobolevn/dotfiles)**  
**[dotfiles using python to install](https://github.com/wkentaro/dotfiles)**  
**[Personal MacOs Workspace Setup](https://hackernoon.com/personal-macos-workspace-setup-adf61869cd79)**  
Step by step on how to install all the essentials.  
Need to take the mas (appstore) automation  
**[bootstrap script example](https://github.com/dvlden/mac-setup/blob/master/bootstrap)**  
Example of how to create the one-touch setup

### zsh/antigen specific links
[awesome-zsh-plugins](https://github.com/unixorn/awesome-zsh-plugins)  
use antibody lol: https://getantibody.github.io/  
[antigen repo](https://github.com/zsh-users/antigen)  
[antigenrc to use custom theme](https://github.com/simmsa/dotfiles/blob/master/antigenrc.zsh)  
interesting: [source the antigen script and do all setup in one go](https://github.com/ajh/dotfiles/blob/master/configs/zsh/dot_zshrc)  
[antigen showoff](https://github.com/zsh-users/antigen/wiki/Show-off)  
[zsh-users repo for plugins](https://github.com/zsh-users)  


## my own setup
*This is my own preferences*

install xcode cli and homebrew
```
xcode-select --install
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew upgrade && brew update
```

install zsh and oh my zsh
```
brew install zsh
```
get these plugins to antibody
```
antigen bundle robbyrussel/oh-my-zsh path:plugins/git
zsh-users/zsh-syntax-highlighting
zsh-users/zsh-history-substring-search
djui/alias-tips
caarlos0/zsh-mkc
zsh-users/zsh-completions
```

restruct .zshrc to get antibody plugins and  
install antibody and get these plugins:  
? get antibody on my setup repo

cut zshrc before pulling them down

add packages to brew
```
brew install exa fzf
```

## INSTALL BREW, BRO

clone the rraihansaputra/setup repo and make symlinks to home

get Brewfile and let it install

install casks on these and rebackup Brewfile
```
brew cask install alfred android-file-transfer caffeine coconutbattery disk-inventory-x divvy dupeguru firefox flux flycut google-chrome handbrake handbrakebatch iterm2 karabiner-elements mounty notion postman avibrazil-rdm rescuetime slimbatterymonitor steam steamcmd textexpander textmate transmission transmission-remote-gui visual-studio-code vscodium vlc vlc-webplugin vlcstreamer
```
install quicklook packages
```
brew cask install qlcolorcode qlstephen qlmarkdown quicklook-json qlimagesize webpquicklook suspicious-package quicklookase qlvideo
```
Get .dmgs for these apps:
(move these to cask if possible)
- Google Drive
- Line
- Pushbullet
- TinkerTool
- TinkerTool System
- DNSCrypt
- Yam Display

install pipenv, create ~/jup, install jupyterlab