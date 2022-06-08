# Installation script for Arch Linux
Do whatever you want with this, it's just a bunch of commands.

This is for Arch Linux installation in a Generation 2 Hyper-V VM. Use at your own risk, any destruction of data on physical hardware is on you, the user of this script.

Installs minimum for Arch to work

Requires user intervention for root password and hostname

INFO:

DISK: GPT, 128 MiB (2MiB-130MiB) EFI FAT32, REST-OF-DISK MiB (130MiB-100%) Linux Filesystem ext4

PACKAGES: base linux-hardened linux-firmware nano networkmanager grub efibootmgr

Timezone: America/Godthab

Keyboard layout: Danish/dk

LOCALE: US English/en_US.UTF-8

How to use:

Boot to Arch Linux installation media

bash <(curl -s https://raw.githubusercontent.com/Greenlandicsmiley/InstallationScriptforArchLinux/main/Install) -s option = silent mode

OR shortened URL

bash <(curl -Ls https://git.io/JtBjP) s option = silent mode, L option = follows shortened URL
