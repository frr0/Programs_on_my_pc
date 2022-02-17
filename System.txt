# Upgrade

sudo dnf update
sudo dnf upgrade

# Upgrade to the newest version

sudo dnf -y update
sudo dnf install dnf-plugin-system-upgrade
sudo dnf system-upgrade download –releasever=INSERT NUMBER
sudo dnf system-upgrade reboot
