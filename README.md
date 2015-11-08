# arch-linux-anywhere
You can find the official Arch Linux Anywhere ISO at:
https://sourceforge.net/projects/arch-anywhere/

Arch Linux Anywhere is an Arch Linux ISO, and installer, which allows you to install Arch regardless of the status of your network connection. I have remastered the official archiso to include local package repos for both respective arcitectures (x86_64 and i686).

These local package repos allow you to proform a full base / base-devel install directly from the ISO. Not only is it a full base / base-devel repo, but it also contains all of the following packages for both arcitectures:

Graphics and desktops: \n

xorg-server xorg-server-utils xorg-xinit xterm
xfce4
awesome
openbox
i3
dwm
xf86-video-ati
nvidia nvidia-340xx nvidia-304xx
xf86-video-intel
virtualbox-guest-utils
lightdm
lightdm-gtk-greeter

Bootloader:

grub
os-prober

network utils:

wireless_tools
wpa_supplicant
netctl
wpa_actiond

Additional optional programs:

arch-wiki
screenfetch
openssh
firefox
htop
zsh
conky
htop
lynx
pulseaudio
cmus

All of these packages are contained within the ISO, effectively allowing you to install Arch Linux Anywhere, without being connected to the internet.

My ISO also contains a built in installer script I've written in shell. This sctipt can be invoked by simply typing arch-installer after booting into the Arch Anywhere ISO.

My script determines the status of your network connection. If you do not have an active connection to the interent it will automatically install the packages from the local repo. However if you do have an active connection it asks to download all the packages from the official repos, while still giving you the choice of downloading locally.

If you are connected to the internet and you choose to install from the official repos you will be given the option to install the additional desktops of your choice:

mate
lxde
lxqt
cinnamon
gnome
kde plasma
enlightenment
fluxbox

The online install also offers a longer list of additional optional software to be included with your Arch Linux install, all from the official repos.
