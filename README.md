# Linux-Termux
To start you need install termux from oficial Termux github Repository

Link:  https://github.com/termux/termux-app/releases

# Commands

List of commands to install Debian in Termux


-------------------------PROOT-DISTRO-------------------------

```bash pkg update
```bash pkg install proot-distro
proot-distro install debian
proot-distro login debian



-------------------------DEBIAN-------------------------



apt update -y

apt install sudo nano adduser -y

adduser {Your user}

nano /etc/sudoers

# Add the following line to the file
droidmaster ALL=(ALL:ALL) ALL

sudo whoami 



-------------------------DESKTOPS-------------------------
# Commands: 
proot-distro login debian --user {Your user}

sudo apt install dbus-x11 nano gnome gnome-shell gnome-terminal gnome-tweaks gnome-software nautilus gnome-shell-extension-manager gedit tigervnc-tools gnupg2 -y

for file in $(find /usr -type f -iname "*login1*"); do rm -rf $file
done



-------------------------TERMUX-X11-------------------------
pkg update

pkg install x11-repo

pkg install termux-x11-nightly

pkg install pulseaudio



# Download the script to Termux
chmod +x startxfce4_debian.sh
./startxfce4_debian.sh
