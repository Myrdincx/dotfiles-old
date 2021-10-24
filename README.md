### These are all my dotfiles :>

## Information about the dotfiles.

These dotfiles are modified, I simply changed a few shortcuts and used compton instead of rofi because of some errors I had with my system.

You can check the [original creator](https://github.com/Manas140/dotfiles) here.

The original dotfiles have 3 configurations for AwesomeWM, BSPWM and I3.

*This repository only includes modifications made to the AwesomeWM configuration.*

---

## Menu

### Installation 

[![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](#debian)

[![ArchLinux](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white)](#arch)


---

## Debian

**SETUP**

We will start with installing a few things that we will need to make the system work.

```
sudo apt install git python3 python3-pip kitty awesome bpytop bspwm cava dunst i3 nautilus polybar ranger rofi zathura picom compton snapd i3lock xclip qt5-style-plugins materia-gtk-theme lxappearance xbacklight flameshot nautilus xfce4-power-manager pnmixer network-manager-gnome policykit-1-gnome feh
```

The dotfiles will need a few extra directories on your pc.
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

**INSTALLATION**\
We first have to make sure that the install command is an executable.\
We can do this by using the chmod command.
```
sudo chmod +x install.sh
```
Now we can install the script with the following command.

```
./install.sh 
```

If you get any errors based on folders not being there.
Check if you actually created them, as said before.





