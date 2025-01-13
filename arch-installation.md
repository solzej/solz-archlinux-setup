# Install

Update & Upgrade Arch
```
sudo pacman -Syu
```

Reboot the system
```
sudo reboot
```
- Install Vulkan driver **(AMD Only)**
```
sudo pacman -S vulkan-radeon lib32-vulkan-radeon
```

- Install Vulkan driver **(NVIDIA Only)**
```
sudo pacman -S nvidia-utils lib32-nvidia-utils
```

- Install packages (official repository)
```
pacman -S chromium base-devel git flatpak steam gamemode wine-staging fastfetch htop btop 
```
- Install Yay - AUR Helper (community repository)
```
git clone https://aur.archlinux.org/yay.git ~/yay
cd ~/yay
makepkg -si --noconfirm
```

- Install packages (community repository) <sup>***optional***</sup>
```
yay -S --noconfirm protonplus 
```

- Disable File Indexer (KDE Only) <sup>***optional***</sup>
```
balooctl suspend && balooctl disable && balooctl purge
```
- Install latest Mesa Driver **(AMD Only)**
```
git clone https://github.com/Frogging-Family/mesa-git.git ~/mesa-git
cd ~/mesa-git
yes | makepkg -si
```
