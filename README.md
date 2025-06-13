<p align="center">
  <a href="https://github.com/Jona1302/My-Dotfiles?tab=readme-ov-file#Installation">Installation</a>
</p>

<p align="center">
  <a href="https://github.com/Jona1302/My-Dotfiles/blob/main/README.md#Hintsheet">Hintsheet</a>
</p>

<p align="center">
  <a href="https://github.com/Jona1302/My-Dotfiles/blob/main/README.md#Bugs">Bugs</a>
</p>

## Installation ##

**1.First we have to install some dependencies:**

- Pacman:
  
      sudo pacman -S kitty firefox thunar ttf-meslo-nerd curl wget zsh swww waybar git python3 bluez-utils brightnessctl pipewire pipewire-pulse ttf-jetbrains-mono-nerd wireplumber

 - yay:

       yay -S waypaper-git pfetch rofi-lbonn-wayland-git bluetui
* If you dont have yay installed, [Click me](https://github.com/Jguer/yay) after you followed this guide you can delete the yay folder
  
  - Or just run this(thats from the website)
    
             sudo pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si

<br/>

**2.Now clone the repos:**

 - my repo
    
       git clone https://github.com/Jona1302/My-Dotfiles.git

- oh-my-zsh
     
      sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
       
- powerlevel10k

      git clone --depth=1 https://github.com/romkatv/powerlevel10k.git "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k"

<br>

**3. Now we have to remove the existing files:**

       rm -rf ~/.config/hypr \
              ~/.config/kitty \
              ~/.config/rofi \
              ~/.config/waybar \
              ~/.zshrc \
              ~/.p10k.zsh    
 
<br>
<br>

**4. Now we can move the new files to the .Config directory**

!!!MAKE SURE THAT YOU ARE IN THE (MY-DOTFILES) DIRECTORY!!!

         cp -r hypr/ kitty/ rofi/ waybar/ ~/.config/ && \
         cp .p10k.zsh .zshrc ~/


**5. At the next step we have to modify the waybar scripts by running this:**

- modifiy

      chmod +x ~/.config/waybar/scripts/*

**6. Last but no least we have to chainge the shell from bash to zsh by running:**

- change shell

      sudo chsh -s $(which zsh)


## Hintsheet ##

 | keybind       | Description              
|----------------|-----------------------------
| WIN + A        | Rofi Launcher              
| WIN + Q        | Terminal(Kitty)           
| WIN + F        | FileManager(thunar)        
| WIN + C        | Close Acitive Window      
| WIN + W        | ChaingeWallpaper            
| WIN + V        | fullscreen a window         
| Win + leftklick| Drag a window               
| Esc            | cloes mini windows like rofi

