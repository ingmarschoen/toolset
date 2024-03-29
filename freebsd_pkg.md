# Install FreeBSD

## Base configuration
Using "German (accent keys)” keyboard layout.
Optional system components
- NO base-dbg
- NO kernel-dbg
- NO lib32-dbg
- lib32
- ports
- NO src
- NO test

## Disk and network
Partition disk using “Auto ZFS” ; and enable root encryption.
Network access via em0.

## System configuration
- NO local_unbound
- sshd
- moused
- ntpdate
- ntpd
- powerd
- NO dumpdev

## Security hardening options
- clear_tmp
- disable_syslogd
- disable_sendmail

## More
Add a user and join the “wheel” group.
Install a local copy of the Handbook.

When it's all done, exit the installer and reboot the system.



# Init working environment
vim
w3m
doas
git
tmux

# Clone dotfiles
git clone ...

# Install X
xorg
drm-kmod libva-intel-driver xf86-video-intel

# More
keepassxc
libyubikey
u2f-devd
pw group mod u2f -m schoen

veracrypt
fusefs-libs3
exa
hs-pandoc
owncloudclient
bash

# /boot/loader.conf
kern.vty=vt
fusefs_load="YES"
autoboot_delay="2"
loader_logo="none"
