First you have to clone my repo:

<pre>git clone https://github.com/Jona1302/My-Dotfiles.git
    
cd My-Dotfiles  </pre>

Next we have to install some dependencys:

Pacman:
<pre> sudo pacman -S swww waybar rofi python3 bluetui bluez-utils brightnessctl pipewire pipewire-pulse ttf-jetbrains-mono-nerd wireplumber </pre>

yay:
<pre>yay -S waypaper-git rofi-lbonn-wayland-git </pre>
if you dont have yay installed, [Klick me](https://github.com/Jguer/yay)



Now we have to remove the existing files:
Hypr:
<pre> sudo rm -rf ~/.config/hypr </pre>

Kitty(if installed):
<pre> sudo rm -rf ~/.config/kitty </pre>

Rofi:
<pre> sudo rm -rf ~/.config/rofi </pre>

Waybar:
<pre> sudo rm -rf ~/.config/waybar </pre>


Now we can move the new files to the .Config directory
<pre> cd ~/home</pre>

Hypr:
<pre> sudo rm -rf ~/.config/hypr </pre>

Kitty(if installed):
<pre> sudo rm -rf ~/.config/kitty </pre>

Rofi:
<pre> sudo rm -rf ~/.config/rofi </pre>

Waybar:
<pre> sudo rm -rf ~/.config/waybar </pre>
