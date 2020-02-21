sudo pacman-mirrors -f0 && sudo pacman -Syyu

Enable AirpodPro in Manjaro
# sudo vi /etc/bluetooth/main.conf
Un-Comment:
ControllerMode = bredr
Restart Bluetooth:
sudo systemctl restart bluetooth

Install Libvirt in Manjaro:
LC_ALL=C lscpu | grep Virtualization
zgrep CONFIG_KVM /proc/config.gz
sudo pacman -S virt-manager qemu vde2 ebtables dnsmasq bridge-utils openbsd-netcat
sudo systemctl enable libvirtd.service
sudo systemctl start libvirtd.service
