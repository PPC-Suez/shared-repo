## Install zsh
```
sudo apt update && sudo apt upgrade -y
sudo apt install zsh-autosuggestions zsh-syntax-highlighting zsh -y
```
-----------------------------------------------------------------------------------------------
## Install Oh My zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
-----------------------------------------------------------------------------------------------
## Install and Configure Oh My ZSH Plugins
```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting

git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting

git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete

sed -i 's/plugins=*/plugins=(git sudo web-search gh zsh-autosuggestions zsh-syntax-highlighting fast-syntax-highlighting zsh-autocomplete aws docker)/' ~/.zshrc

sed -i 's/ZSH_THEME=*"/ZSH_THEME=\"fino-time\"/' ~/.zshrc

source ~/.zshrc

clear

```
-----------------------------------------------------------------------------------------------
