### These are all my dotfiles :>

## Information about the dotfiles.

These dotfiles are modified, I simply changed a few shortcuts and used compton instead of rofi because of some errors I had with my system.

You can check the [original creator](https://github.com/Manas140/dotfiles) here. *note: they have changed their dotfiles, so they dont really look alike anymore*

The original dotfiles have 3 configurations for AwesomeWM, BSPWM and I3.

*This repository only includes modifications made to the AwesomeWM configuration.*

---

## Menu

### Installation 

[![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](#debian)

- [Setup](#setup-)
- [Installation](#installation-)
- [Fixing problems and bugs](#fixing-problems-and-bugs-)
- [Installing extra tools (optional)](#installing-extra-tools-optional-)

[![ArchLinux](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white)](#arch)

- [Setup](#setup--1)
- [Installation](#installation--1)
- [Fixing problems and bugs](#fixing-problems-and-bugs--1) 
- [Installing extra tools (optional)](#installing-extra-tools-optional--1) - Adding soon

[![ArchLinux](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white)](#important-keybinds-)
[![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](#important-keybinds-)
- [Important keybinds](#important-keybinds-) - Adding soon

_**FUTURE FIXES CAN BE ADDED**_
---

## Debian [🔝](#menu)

### SETUP [🔝](#menu)

We will start with installing a few things that we will need to make the system work.

```
sudo apt install git python3 python3-pip kitty awesome bpytop bspwm cava dunst i3 nautilus polybar ranger rofi zathura picom compton snapd i3lock xclip qt5-style-plugins materia-gtk-theme lxappearance xbacklight flameshot nautilus xfce4-power-manager pnmixer network-manager-gnome policykit-1-gnome feh
```

The dotfiles will need a few extra directories on your pc.\
We can easily create those in case they aren't there yet.

```
mkdir ~/.fonts
mkdir ~/Pictures/Wallpapers
mkdir ~/.local/bin/
```

We will also have to download this repository.\
I prefer the Download folder for this.\
To do this, make sure you are in the *home* directory.

*The following command will create a git folder inside of the Download folder*\
*It will download the repository right after, and cd into it.*

```
cd Downloads
mkdir git
cd git
git clone https://github.com/Myrdincx/dotfiles.git && cd dotfiles
```

### INSTALLATION [🔝](#menu)
We first have to make sure that the install command is an executable.\
We can do this by using the chmod command.
```
sudo chmod +x install.sh
```
Now we can install the script with the following command.

```
./install.sh 
```

If you get any errors based on folders not being there.\
Check if you actually created them, as said before.

**Now log-out and log back into AwesomeWM**

### FIXING PROBLEMS AND BUGS [🔝](#menu)

The main problem will probably be Polybar. \
We first have to make sure that the polybar launch.sh is an executable.\
Make sure you are in the home directory.
```
cd .config
chmod +x launch.sh
chmod +x updates.sh
./launch.sh
```
You will probably see a few errors.\
These can be fixed in the modules.ini file.\
You can access the file by the following command.\
Make sure you are in the Polybar directory.
```
nano modules.ini
```
After fixing everything, press the following keys.\
*MOD + SHIFT + R*

### INSTALLING EXTRA TOOLS (OPTIONAL) [🔝](#menu)

We now have the base installation of the system, we can now start installing some extra tools if wanted.\
I'm going to show you how to install the following tools.

Tools | What they do
------------ | -------------
ranger | File manager accessible in the Terminal 
bpytop | A cool looking htop alternative
snapcraft | Package installer
snapcraft Discord | Discord installed with the snapcraft package installer
Manas140 SH scripts | A bunch of SH scripts made by [Manas140](https://github.com/Manas140/sh)
Manas140 Fetch script | A simplistic fetch script made by [Manas140](https://github.com/Manas140/fetch)
Manas140 Pluck script | A simplistic Color Picker script made by [Manas140](https://github.com/Manas140/pluck)

**Ranger**
```
sudo apt install ranger
```

**bpytop**
```
sudo apt install bpytop
```

**Snapcraft**
```
sudo apt update
sudo apt install snapd
snap install core
```

**Snapcraft Discord**
```
sudo snap install discord
```

**Manas140 SH scripts**
```
git clone https://github.com/manas140/sh.git && cd sh
sudo ./install.sh i
```
**Manas140 Fetch script**
```
git clone https://github.com/Manas140/fetch.git && cd fetch
./install.sh i
```
**Manas140 Pluck script**
```
sudo apt install xinput xdotool imagemagick libnotify-bin xclip
mkdir /tmp/pluck
git clone https://github.com/Manas140/pluck.git && cd pluck
./install.sh i
```

## Arch [🔝](#menu)

### SETUP [🔝](#menu)

We will start by installing a few things that we will need to make the system work.\
Make sure you have git installed, if this is not the case please follow the following instruction.
```
sudo pacman -S git
```
We are now able to install YAY.
```
cd Downloads
mkdir git && cd git
sudo git clone https://aur.archlinux.org/yay.git
sudo chown -R  <nameofuserhere>:users yay
cd yay
makepkg -si
```
Now that yay is installed, we can continue installing the rest of things we need.
```
yay -S git python3 kitty awesome bpytop bspwm cava dunst i3 nautilus polybar ranger rofi zathura picom compton snapd i3lock-fancy xclip qt5-styleplugins materia-gtk-theme lxappearance flameshot nautilus xfce4-power-manager pnmixer network-manager-applet feh ttf-roboto polkit-gnome 
```
The dotfiles require you to have a few folders on your pc.\
We can easily create them with the following command.
```
mkdir ~/.fonts
mkdir ~/Pictures/Wallpapers
mkdir ~/.local/bin/
```
We will also have to download this repository in order to use it.\
I prefer the download folder with a git folder in there.\
To do this, make sure you are in the home directory.

*The following command will create a git folder inside of the Download folder
It will download the repository right after, and cd into it.*
```
cd Downloads
mkdir git
cd git
git clone https://github.com/Myrdincx/dotfiles.git && cd dotfiles
```

### INSTALLATION [🔝](#menu)

We first have to make sure tht the install command is an executable.
We can do this by using the chmod command.

```
sudo chmod +x install.sh
```
Now, we can install the script with the following command.

```
./install.sh 
```
If you get any errors based on folders not being there.\
Check if you actually created them, as said before.

**Now log-out and log back into AwesomeWM**

### FIXING PROBLEMS AND BUGS [🔝](#menu)

The main problem will probably be Polybar.\
We first have to make sure that the Polybar is installed and that the launch.sh is an executable.\
```
yay -S polybar
```
Make sure you are in the home directory.
```
cd .config
cd polybar
chmod +x launch.sh 
chmod +x updates.sh
./launch.sh
```
You will probably see a few errors.\
These can be fixed easily.\
We will first change the update.sh file.\
*Make sure you are in the Polybar folder.*
```
nano updates.sh

Now remove the apt update
```
You can also change modules by editing the modules.ini file.
```
nano modules.ini
```
After fixing everything, press the following keys to restart AwesomeWM.
*MOD + SHIFT + R*


### INSTALLING EXTRA TOOLS (OPTIONAL) [🔝](#menu)

**Coming Soon**


## IMPORTANT KEYBINDS [🔝](#menu)


**Coming Soon**
