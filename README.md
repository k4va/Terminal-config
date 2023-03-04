# TERMINAL CONFIG
In this repository have my configs for a Linux terminal.

I am using a zsh as shell, kitty as terminal and different plugins for most detail and easy use.

## Kitty installation
For Debian/Ubuntu based systems can be installed from apt repositories using:

```bash
sudo apt install kitty
```

For Arch based systems use pacman repositories:

```bash
sudo pacman -S kitty
```

## Kitty Configs

To configure Kitty, copy the files in the folder [kitty](kitty) (color.ini and kitty.conf) in the rute `~/.config/kitty`

## Zsh installation

To install zsh and plugins in Debian/Ubuntu based systems can be installed from apt.
The plugins are zsh-syntax-highlighting and zsh-autosuggestions:

```bash
sudo apt install zsh zsh-syntax-highlighting zsh-autosuggestions
```

To Arch based systems can be installed using pacman:
```bash
sudo pacman -S zsh zsh-syntax-highlighting zsh-autosuggestions
``` 

To enable zsh as shell follow next commands:
```bash
sudo su
usermod --shell /usr/bin/zsh user
usermod --shell /usr/bin/zsh root

#Symlink of root zshrc to user's zshrc
ln -s -f /home/kava/.zshrc /root/.zshrc

```

## Zshrc configuration

The configuration of ZSHRC it's find in the file [.zshrc](.zshrc)

## Extra plugins
As plugins extra, i use Lsd and bat.

To Debian/Ubuntu can be download Lsd [here](https://github.com/Peltoche/lsd)

And Bat [here](https://github.com/sharkdp/bat)

To install zsh sudo plugin:

```bash
cd /usr/share
sudo mkdir zsh-plugins
sudo chown usuario:usuario zsh-plugins
cd zsh-plugins
wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/plugins/sudo/sudo.plugin.zsh
```

To Arch can be installed using pacman:
```bash
sudo pacman -S lsd bat
```

# Zsh Theme and Font

As font i use Mononoki Nerd Font from site [nerdfonts.com](nerdfonts.com) and theme is powerlevel10k, can be installed from [here](https://github.com/romkatv/powerlevel10k).

# Additional programs
``` bash
sudo apt install xclip
sudo pacman install xclip
```
