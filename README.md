### Installing yay
Yay (Yet Another Yogurt) is AUR helper 
```
sudo pacman -S git
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```

### VS Code configuring
First of all, installing VS Code:
```
yay -S visual-studio-code-bin
```
Then open it and replace *settings.json* and *keybindings.json*

If you need to merge menu bars set **window.title.BarStyle** to *custom* instead of *native*

### Bluetooth enabling
```
yay -S bluez
sudo systemctl start bluetooth.service
sudo systemctl enable bluetooth.service
```

### Anaconda installing
```yay -S acaconda```

If *“conda: command not found”* add conda to *PATH*
```echo "export PATH="/opt/anaconda/bin:$PATH" >> ~/.bashrc```


### Some useful packages
Implementation of Office: ```onlyoffice-bin``` 
2-factor authentication: ```authy```

Video player: ```mpv```
Audio player: ```byte```
Photo viewer: ```gwenview```