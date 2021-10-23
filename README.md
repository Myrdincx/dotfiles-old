### These are all my dotfiles :>

## Short information about the dotfiles.

Most of the dotfiles are created by other people.\
I mostly changed some stuff like shortcuts, extra tools, ...

**The Original DOTS are for BSPWM, AWESOMEWM and I3, but I prefer AWESOMEWM**
*Dotfiles will only include changes to the AWESOMEWM configuration*

---

## Installation

First of all, you will need some tools, depending on your OS, you will have to follow different steps.\
This repo will contain instructions for DEBIAN based systems and ARCH based systems.



### Debian:
First we will install everything we need.

```
sudo apt install git python3 python3-pip kitty awesome bpytop bspwm cava dunst i3 nautilus polybar ranger rofi zathura picom compton
```
Now, clone the repo with the followign command.

```
cd Downloads
mkdir git && cd git
git clone https://github.com/Myrdincx/dotfiles.git
```

After this, logout and change to Awesome.
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

## Make changes 

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

