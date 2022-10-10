## easyi3 ##

This script is intended to be used on a headless Arch or Debian based distribution.

The end result being an i3 window manager with all it's depend's, a torrified ZSH shell with network monitoring, work load balancing, an advanced intrusion detection system and general performance enhancements set by default.

ZSH syntax highlighting and autocorrect are set up aswell as alias's for bleachbit and system matinence:

Bleachbit as user:

```BASH
clean
```

Bleachbit as root:

```BASH
deep-clean
```

Update package manager cache and remove unused packages:

```BASH
rolling
```

Aswell as global alias's for:

Alias | Command |
| --- | --- |
p | python3 |
b | bash |
tab | xfce4-terminal --tab |
c | clear && |
x | rm -rf ~/zsh_history ; history -c |
cx | rm -rf ~/zsh_history ; history -c ; rm - rf .local/share/recently-used.xbel && clear |

Wallpapers are sourced from your ~/Pictures folder making it quick and easy and Rofi was made transparent and full screen to maximize screen space.

The packages will vary depending on your distro:

Package | Arch | Debian | Syslinked |
| --- | --- | --- | --- |
i3 meta | y | y | n |
lightdm | y | y | y |
git | y | y | n |
trash-cli | y | y | n |
axel | y | y | n |
fail2ban | y | y | y |
zsh | y | y | n |
memcached | y | y | y |
memlockd | n | y | y |
xfce4-terminal | y | y | y |
tor | y | y | y |
brightnessctl | y | y | n |
tuned | y | y | y |
ufw | y | y | y |
auditd | y | y | y |
thunar | y | y | n |
rofi | y | y | n |
feh | y | y | n |
tlp | y | y | y |
firefox | y | n | n |
unburden-home-dir | n | y | n |
nocache | n | y | n |
curl | y | y | n |
network-manager-openvpn-gnome | n | y | n |
network-manager-openvpn-pptp | n | y | n |
macchanger | n | y | y |
apt-transport-tor | n | y | n |

A desktop item will be created in '/etc/xdg/autostart/' that automatically sets your CPU Frequency Governor to 'Performance' mode.

Lastly, this script will curl/wget two other packages I find highly-useful/essential:

<div>
  <html>
  <a href="https://github.com/soimort/translate-shell">Translator</a>
  <a href="https://github.com/sdushantha/tmpmail">Tmpmail</a>
  </html>
</div>



***

## On Debian ##

When the install script is run it authors a second script in your home folder called 'root.' When this script is run as root it will compress your bootloader using lz4 and z3fold- which makes for faster boot times. It is not necessary to run this script. However, easyi3 will attempt to. This function is still in testing and *might* not work. If so simply terminate the program- all of the heavy work will be done by then- then run:

```BASH
su root
bash root
```

## On Arch ##

There is no root script. I'm assuming if you are on Arch you can manage your own kernel.

***

## To use ##

First, download and install of any Headless Arch or Debian based distribution then establish a network connection. Install git by running

```BASH
sudo pacman -Ss git || sudo apt install git
```

Then run:

```BASH
git clone https://www.github.com/ZZZlax/easyi3 && cd easyi3 && bash easyi3
```

The script should begin with either

>> Setting up keyring

or

>> Updating apt cache

If you try to run easy i3 on a distro that doesn't use apt or pacman the script will fail. Feel free to install the packages listed one by one and list which ones are available for your distribution and join the in!

Thanks, hope this helps!
