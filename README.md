### These are all my dotfiles :>

## Short information about the dotfiles.

Most of the dotfiles are created by other people.\
I mostly changed some stuff like shortcuts, extra tools, ...

**The Original DOTS are for BSPWM, AWESOMEWM and I3, but I prefer AWESOMEWM**\
*Dotfiles will only include changes to the AWESOMEWM configuration*

---

## Installation

First of all, you will need some tools, depending on your OS, you will have to follow different steps.\
This repo will contain instructions for DEBIAN based systems and ARCH based systems.



### Debian:
First we will install everything we need.

```
sudo apt install git python3 python3-pip kitty awesome bpytop bspwm cava dunst i3 nautilus polybar ranger rofi zathura picom compton snapd i3lock xclip qt5-style-plugins materia-gtk-theme lxappearance xbacklight flameshot nautilus xfce4-power-manager pnmixer network-manager-gnome policykit-1-gnome 

```
Now, clone the repo with the followign command.

```
cd Downloads
mkdir git && cd git
git clone https://github.com/Myrdincx/dotfiles.git
```

After this, logout and change to Awesome.\
Now you can enter the system using AwesomeWM. 

**Interesting shortcuts**
```
MOD + SHIFT + R -  Restart Awesome
MOD + X - Open Terminal (Kitty)
MOD + E - Open Nautilus (File explorer)
MOD + B - Open Browser (Firefox by default)
```

### Arch:

**ADDING SOON**

---

**Possible Bugs and Fixes**

There is a possibility that your polybar will not show.
First of all try to run the polybar command by going into the folder and launching it.
*Make sure you are in the home directory*

```
cd .config
cd polybar
./launch.sh
```
If this fails, you might have to make launch.sh an executable.
```
sudo chmod +x launch.sh
```
Now try to run the command again.

** Polybar error message**
You might get an error message when the polybar launches, to fix this try to configure the updates.sh file.
```
cd .config
cd polybar
nano updates.sh

*remove the xbps-install -Mun and replace with:
apt update
```
Now press *MOD + SHIFT + R* to restart AwesomeWM

---

## Make changes and configuring things

**You are able to make changes to the files and theme in AwesomeWM.**

Make sure you are in the home directory.

```
cd .config
cd awesome
ls -a

*Now you are able to change things by using nano or vim*

nano keys.lua
nano rc.lua
```

Install for example Discord with SNAPSTORE
```
sudo snapd install discord
```


