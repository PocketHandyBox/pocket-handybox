PocketHandyBox Portable Linux with NVIDIA drivers OOTB (Based on Debian 12 and Porteus Initrd)
(now in active development)

Based on Debian 12 and Devuan

Porteus Initrd, overlayfs, sysvinit (build with systemd is possible too), Xfce 4.18

Includes applications such as CPU-X, GSmartControl, GParted, Partimage, Partclone,
TestDisk, ddrescue, WHDD.

Both UEFI and Legacy/CSM boot modes supported. Ventoy compatible (minimal version 1.0.80)
Support boot from USB/SATA/NVMe devices, from FAT32/exFAT/Ext2/3/4/NTFS filesystems.
Secure Boot is not supported and must be disabled.

Contains three versions of NVIDIA proprietary GPU drivers - current 550.x,
and legacy 390.x and 340.x. At boot time, the 'linuxrc' script automatically
determines which driver squashfs module to load.

The default boot option is 64bit Linux 6.10 kernel. NVIDIA 550.x and 390.x
driver modules are pre-built.

Additionally, a 64bit Linux 5.10 kernel is supplied. It must be selected if a legacy 340.x
NVIDIA driver is required (390.x is also pre-built). This kernel uses the Broadcom WL
WiFi driver for 802.11n adapters, which do not work with free drivers.

Linux 5.10 kernel built with intel-nvme-remap patch from EndlessOS to make NVMe SSDs
available on 6th-10th gen Intel Core i3/i5/i7 platforms with "Intel RST Premium With Optane"
option enabled in UEFI Setup.

Download Releases
https://github.com/PocketHandyBox/pocket-handybox/releases

Forum threads
[EN] https://forum.puppylinux.com/viewtopic.php?t=13647
[RU] https://forum.puppyrus.org/index.php?topic=24381.0

Thanks to Fred (fredx181) from forum.puppylinux.com
Developer of DogLinux project https://debiandog.github.io/doglinux/
