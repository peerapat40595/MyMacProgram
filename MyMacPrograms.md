# System Preferences
# Keyboard
#	- Fn key
#	- Lang
# Start up program
#	- User

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

brew cask install iterm2

# http://sourabhbajaj.com/mac-setup/iTerm/zsh.html


brew install zsh zsh-completions

brew install nvm
# -> add sth in ~/.zshrc
echo 'export NVM_DIR="$HOME/.nvm"' >> ~/.zshrc
echo '. "/usr/local/opt/nvm/nvm.sh"' >> ~/.zshrc

brew install tree

brew install autojump
echo '[ -f /usr/local/etc/profile.d/autojump.sh ] && . /usr/local/etc/profile.d/autojump.sh' >> ~/.zshrc

brew cask install alfred
brew cask install shiftit
brew cask install firefox
brew cask install docker
brew cask install visual-studio-code
brew cask install intellij-idea
brew cask install cleanmymac
brew cask install sublime-text

install XCode
sudo xcode-select -s /Applications/Xcode.app/Contents/Developer

# https://teamgaslight.com/blog/vim-plus-tmux-a-perfect-match
brew install tmux
brew install python
export PATH="/usr/local/opt/python/libexec/bin:$PATH"
brew install macvim --with-override-system-vim