<p align="center">
 
 [Install](https://github.com/Jona1302/My-Dotfiles#setup)
</p>

## Setup ##

**1.First we have to install some dependencys:**

- Pacman:
  
      sudo pacman -S kitty firefox thunar ttf-meslo-nerd curl wget zsh swww waybar git python3 bluez-utils brightnessctl pipewire pipewire-pulse ttf-jetbrains-mono-nerd wireplumber

 - yay:

       yay -S waypaper-git pfetch rofi-lbonn-wayland-git bluetui
* If you dont have yay installed, [Klick me](https://github.com/Jguer/yay) after you followed this guide you can delete the yay folder

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

 - Hypr:
 
        sudo rm -rf ~/.config/hypr 

 - Kitty(if installed):
 
        sudo rm -rf ~/.config/kitty

  - Rofi:
 
        sudo rm -rf ~/.config/rofi

  - Waybar:

        sudo rm -rf ~/.config/waybar

  - pw10k:

        sudo rm ~/.zshrc

    
  - zshrc:

        sudo rm ~/.p10k.zsh

    

<br>
<br>

**4. Now we can move the new files to the .Config directory**

!!!MAKE SURE THAT YOU ARE IN THE (MY-DOTFILES) DIRECTORY!!!

- Hypr:
 
      cp -r hypr/ ~/.config/
  
- Kitty(if installed):
 
      cp -r kitty/ ~/.config/

- Rofi:
 
      cp -r rofi/ ~/.config/

- Waybar:

      cp -r waybar/ ~/.config/

- pw10k:

      cp .p10k.zsh ~/

- zshrc:

      cp .zshrc ~/

**5. At the next step we have to modify the waybar scripts by running this:**

- modifiy

      chmod +x ~/.config/waybar/scripts/*

**6. Last but no least we have to chainge the shell from bash to zsh by runnig:**

- chainge shell

      sudo chsh -s $(which zsh)
