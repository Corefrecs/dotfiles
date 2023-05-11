# dotfiles

## Using this repository
~~~
git clone --bare https://github.com/Corefrecs/dotfiles.git ~/.dotfiles 
alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
config checkout -> if errors occure, backup or delete the conflicting files
~~~
Done! Now you can work with the "config" command like:
~~~
config status
config add XY 
config commit -m "this is a description"
config push
~~~
To commit changes in tracked files, use:
~~~
config commit -am "Update"
~~~

## Pakages for Sway
sway swaybg swayidle waybar autotiling-rs wofi foot dolphin kate firefox polkit-kde-agent mako kvantum qt5ct ttf-jetbrains-mono-nerd git base-devel github-cli

## Pakages for Hyprland
hyprland kitty xorg-xwayland dolphin firefox wofi grim slurp pavucontrol mesa mako xdg-desktop-portal-hyprland polkit-kde-agent qt5-wayland qt6-wayland qt5ct kvantum hyprpaper ttf-jetbrains-mono-nerd swayidle git base-devel github-cli

- AUR
waybar-hyprland

## Environment variables, some are global, some are for sway. NOT NEEDED FOR HYPRLAND!
~~~
MOZ_ENABLE_WAYLAND=1 firefox
MANGOHUD=1
ENABLE_VKBASALT=1
QT_QPA_PLATFORMTHEME=qt5ct
QT_QPA_PLATFORM=wayland
~~~
