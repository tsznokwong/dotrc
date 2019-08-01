dotrc
===

# Setup
## vim
```
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

brew install cmake
vim +PluginInstall +qall
.vim/bundle/YouCompleteMe/install.py --clang-completer
cmake -G "Unix Makefiles" -DPATH_TO_LLVM_ROOT=~/ycm_temp/llvm_root_dir . ~/.vim/bundle/YouCompleteMe/third_party/ycmd/cpp
cmake --build . --target ycm_core --config Release
```
## iTerm2
```
brew cask install iterm2

brew install zsh zsh-completions
sudo sh -c "echo $(which zsh) >> /etc/shells"
chsh -s $(which zsh)
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

git clone git://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
open $ZSH_CUSTOM/plugins/zsh-autosuggestions/zsh-autosuggestions.zsh {ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE='fg=240'}

brew install zsh-syntax-highlighting

open ~/.zshrc {ZSH_THEME="bullet-train", font=Powerline fonts@GitHub,meslo}
```

# Tools
## vim
1. [Vundle](https://github.com/VundleVim/Vundle.vim.git)
2. [YouCompleteMe](https://github.com/Valloric/YouCompleteMe)

## iTerm2
[iTerm2](https://github.com/gnachman/iTerm2)
1. [zsh](http://www.zsh.org)
2. [zsh-completions](https://github.com/zsh-users/zsh-completions)
3. [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh/)
4. [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
5. [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
6. Theme: [bullet-train](https://github.com/caiogondim/bullet-train.zsh)

# Device
MacBookPro (15", 2017) macOS 10.13.x
