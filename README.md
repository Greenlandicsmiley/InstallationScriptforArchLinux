# Installation script for Arch Linux
Do whatever you want with this, it's just a bunch of commands.

This is for Arch Linux installation in a Generation 2 Hyper-V VM, but will work on any HDD that uses /dev/sdX. Use at your own risk, any destruction of data on physical hardware is on you, the user of this script.

Installs minimum for Arch to work

Only requires user intervention for admin username, admin password, root password and hostname

INFO:

DISK (NO SWAP): GPT, 512 MiB (2MiB-514MiB) EFI fat32, REST-OF-DISK MiB (514MiB-100%) Linux Filesystem ext4

PACKAGES: base base-devel linux-hardened* linux-firmware nano networkmanager** grub efibootmgr

*: Use other kernels if desired

**: Use other network manager if desired. DHCP enabled in chroot, feel free to disable DHCP (rm /etc/NetworkManager/conf.d/dhcp-client.conf) and set static IP

TIMEZONE: Greenland, Nuuk / America/Godthab

LOCALE: US English/en_US.UTF-8

KEYBOARD LAYOUT: Danish/dk

This assumes that there is a DHCP server in the network. If you do not have a DHCP server, then set an IP address before running the script.

How to use:

Boot to Arch Linux installation media

bash <(curl -s https://raw.githubusercontent.com/Greenlandicsmiley/InstallationScriptforArchLinux/main/Install) -s option = silent mode

OR shortened URL

bash <(curl -Ls https://git.io/JtBjP) s option = silent mode, L option = follows shortened URL
