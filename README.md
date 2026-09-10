
## Comandos a ejecutar en la consola de la VM
sudo systemctl set-default multi-user.target

sudo apt purge -y \
task-gnome-desktop \
task-spanish-desktop \
gnome-core \
gnome-shell \
gdm3

sudo apt autoremove --purge -y
sudo apt clean

sudo apt purge -y 'xserver-xorg*'

sudo apt autoremove --purge -y
sudo apt clean

sudo apt purge -y \
cups \
cups-browsed \
avahi-daemon \
modemmanager \
bluetooth \
bluez

sudo apt autoremove --purge -y
sudo apt clean

sudo journalctl --vacuum-time=7d

sudo reboot
