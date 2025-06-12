

 __First we have to install some dependencys:__

 Pacman:
 <pre> sudo pacman -S kitty swww waybar git python3 bluez-utils brightnessctl pipewire pipewire-pulse ttf-jetbrains-mono-nerd wireplumber </pre>

 yay:
 <pre>yay -S waypaper-git rofi-lbonn-wayland-git bluetui </pre>
 if you dont have yay installed, [Klick me](https://github.com/Jguer/yay) after you followed this guide you can delete the yay folder.<br />
 

 Now clone the repo:
 <pre>git clone https://github.com/Jona1302/My-Dotfiles.git </pre>

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

!!!MAKE SHURE THAT YOU ARE IN THE MY-DOTFILES DIRECTORY!!!

 Hypr:
 <pre> cp -r hypr/ ~/.config/ </pre>

 Kitty(if installed):
 <pre> cp -r kitty/ ~/.config/ </pre>

 Rofi:
 <pre> cp -r rofi/ ~/.config/ </pre>

 Waybar:
 <pre> cp -r waybar/ ~/.config/ </pre>

 At the last step we have to modify the waybar scripts by typing this:

  <pre> chmod +x ~/.config/waybar/scripts/* </pre>
