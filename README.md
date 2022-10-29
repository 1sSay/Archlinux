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
```yay -S visual-studio-code-bin```
Then open it and replace *settings.json* and *keybindings.json*

If you need to merge menu bars set window.title.BarStyle to "custon" instead of "native"

### How to enable Bluetooth
```
yay -S bluez
sudo systemctl start bluetooth.service
sudo systemctl enable bluetooth.service
```