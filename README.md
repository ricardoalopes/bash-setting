# bash-setting
Default personal configuration for MacOS Terminal look and feel

## Install ohmyzsh
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Instal ohmyzsh Plugins
```
git clone https://github.com/zdharma/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting
```

``` 
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

```
git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
```

## Install Fonts needed for theme (to display git branch icons)
```
cd ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/themes && git clone https://github.com/powerline/fonts.git --depth=1 && cd fonts && ./install.sh%
```

## Create Symbolic Links for .zshrc and personal-alias file
```
ln -s ${PWD}/.zshrc ~/.zshrc && ln -s ${PWD}/personal-alias ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/personal-alias
```

## Apply Theme in Terminal
solarized-dark-patched.terminal
