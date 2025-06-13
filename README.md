## Setup ##

**1.First we have to install some dependencys:**

- Pacman:

      sudo pacman -S kitty firefox fastfetch swww waybar git python3 bluez-utils brightnessctl pipewire pipewire-pulse ttf-jetbrains-mono-nerd wireplumber

 - yay:

       yay -S waypaper-git rofi-lbonn-wayland-git bluetui
* If you dont have yay installed, [Klick me](https://github.com/Jguer/yay) after you followed this guide you can delete the yay folder

<br/>

**2.Now clone the repo:**

 - git
    
       git clone https://github.com/Jona1302/My-Dotfiles.git

<br>

**3. Now we have to remove the existing files:**

 - Hypr:
 
        sudo rm -rf ~/.config/hypr 

 - Kitty(if installed):
 
        sudo rm -rf ~/.config/kitty

  - Rofi:
 
        sudo rm -rf ~/.config/rofi

  - Waybar:

        sudo rm -rf ~/.config/waybar

<br>


**4. Now we can move the new files to the .Config directory

!!!MAKE SHURE THAT YOU ARE IN THE MY-DOTFILES DIRECTORY!!!

Hypr:
 
    cp -r hypr/ ~/.config/

Kitty(if installed):
 
    cp -r kitty/ ~/.config/

Rofi:
 
    cp -r rofi/ ~/.config/

Waybar:

    cp -r waybar/ ~/.config/

## 5. At the last step we have to modify the waybar scripts by typing this:

    chmod +x ~/.config/waybar/scripts/*
