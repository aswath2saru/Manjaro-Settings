sudo pacman-mirrors -f0 && sudo pacman -Syyu

Enable AirpodPro in Manjaro
``` # sudo vi /etc/bluetooth/main.conf
Un-Comment:
ControllerMode = bredr
Restart Bluetooth:
sudo systemctl restart bluetooth ```
