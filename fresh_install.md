### Initial Requirements

```bash
sudo apt install build-essential
sudo apt install git
sudo apt install suckless-tools
sudo apt install i3status
sudo apt install i3lock
sudo apt install net-tools
sudo apt install fonts-font-awesome acpi # for battery i3blocks
sudo apt install thunderbird
sudo apt install feh
sudo apt-get install fzf
sudo apt install libreoffice
sudo apt install sysstat # for cpu_usage i3blocks
sudo apt install tig
sudo apt install rxvt-unicode
```

### Followed this tutorial https://github.com/k-vernooy/dotfiles
1. install i3-gaps from source
2. install picom as composite manager https://github.com/ibhagwan/picom.git
3. install i3blocks from source https://github.com/vivien/i3blocks#installation


### zsh

- sudo apt install zsh

### lock screen
- follow this tutorial https://github.com/pavanjadhaw/betterlockscreen 
- install i3lock-color


### Back to the ethX names

```bash
sudo gedit /etc/default/grub
# change line GRUB_CMDLINE_LINUX=""    to     GRUB_CMDLINE_LINUX="net.ifnames=0 biosdevname=0" 
sudo update-grub
reboot
```

### manage multiple monitors
git clone --recursive https://github.com/Ventto/mons.git
cd mons
sudo make install

### 256 color terminal - needed for tigrc color scheme
sudo apt-get install rxvt-unicode-256color

-> add `URxvt*termName: rxvt-unicode-256color` to the .XResources file of urxvt