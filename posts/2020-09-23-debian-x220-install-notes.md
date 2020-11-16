---
title: Debian Buster on Thinkpad x220
author: Colton Grainger
date: 2020-09-23
revised:
---

set the mood with [“Future's 'High Off Life' Album (2020)”](https://www.youtube.com/playlist?list=PL9tY0BWXOZFvtPSkcmehO175eN5PU5XMs) 

## old laptop

torrented Debian 10.5 buster 

<https://www.debian.org/releases/stable/debian-installer/>

is it legit?

```
$ md5sum debian-edu-10.5.0-amd64-netinst.iso | grep 3f498829412f4dfb6f43911d957849dc
```

where's my flash media?

```
$ df -h /media/colton/*

Filesystem                    Size  Used Avail Use% Mounted on
/dev/mapper/lobster--vg-root  204G  166G   27G  87% /
/dev/sdb1                     2.6G  2.6G     0 100% /media/colton/
/dev/sdb3                      64Z   64Z   27G 100% /media/colton/
```

burn the iso image

```
$ sudo dd if=$PWD/debian-edu-10.5.0-amd64-netinst.iso of=/dev/sdb && sync

858112+0 records in
858112+0 records out
439353344 bytes (439 MB, 419 MiB) copied, 72.1786 s, 6.1 MB/s
```

opps, forgot firmware <https://packages.debian.org/buster/firmware-iwlwifi>

```
$ wget http://ftp.debian.org/debian/pool/non-free/f/firmware-nonfree/firmware-iwlwifi_20190114-2_all.deb

Resolving ftp.debian.org (ftp.debian.org)... 130.89.148.12
Connecting to ftp.debian.org (ftp.debian.org)|130.89.148.12|:80... connected.
HTTP request sent, awaiting response... 200 OK
Length: 5318404 (5.1M) [application/x-debian-package]

2020-09-23 15:19:37 (506 KB/s) - ‘firmware-iwlwifi_20190114-2_all.deb’ saved [5318404/5318404]
```

what do I need to do with this package? (aptitude already has it on my system, but I need the `*.ucode` fileS)

<https://www.linuxquestions.org/questions/debian-26/how-to-provide-non-free-firmware-files-to-the-debian-jessie-installer-4175542680/>

```
$ dpkg-deb --extract firmware-iwlwifi_20190114-2_all.deb wifi
$ cd wifi/
```

> This step created two new subdirectories: lib and usr.
>
> The lib directory, in turn, contained a further subdirectory, firmware, that held all firmware files extracted from both packages―including, but not limited to, the files that I (or, rather, the Debian installer) was looking for.

```
$ cp iwlwifi-1000-5.ucode /media/colton/flash/
```

> Note, in particular, this [second] USB stick included the contents of the firmware directory, not the directory itself!

## new laptop

fooled around in BIOS menu, 

- disabled anti-theft, 
- left BIOS password settings along (for fear)
- enabled virtualization for installing the liquorix low-latency kernel
- there's a fingerprint scanner! wowowow!

inserted the boot iso image (first USB stick) then

```
Some of your hardware needs non-free firmware files to operate. The firmware can
be loaded from removable media, such as a USB stick or floppy.

The missing firmware files are: iwlwifi-1000-5.ucode ...
````

opps! non-free networking firmware

> Finally, the time had come to retry the Debian installation. I simply booted the computer off the Debian 8.0.0 medium, and when it complained again about the missing firmware files, I took the following steps:
>
> - I inserted the [second] USB stick.
s - I pressed the <CTRL>+<Alt>+<F2> key combination, to switch to the second virtual terminal.
> - I ran the `blkid` command, to find out under which device name the USB stick was known: /dev/sdc. Its [ext4] filesystem, which contained the firmware files, then, was /dev/sdc1.
> - I mounted the filesystem under the /lib/firmware mountpoint―which, however, I had to create first:

```
mkdir /lib/firmware
mount -f ext4 /dev/sdc1 /lib/firmware
```

> - I pressed <CTRL>+<Alt>+<F5> to continue the installation process.
> - The firmware files were successfully loaded, and I got prompted for my wireless networking parameters.

primary network interface

```
enp0s25 <intel gigabit network connection>
wlp3s0 <intel centrino wireless-N 1000>
```

then `ifup` for this wifi connection

then `xorg` and `xmonad` and `libghc-xmonad-dev` and `libghc-xmonad-contrib-dev`

TODO

- fish
    - then $fish_user_path
- firefox-esr
- urxvt
    - https://askubuntu.com/questions/821157/print-a-256-color-test-pattern-in-the-terminal
    - .Xresources
- curl
- UW ttyp0 bitmap fonts
    - https://people.mpi-inf.mpg.de/~uwe/misc/uw-ttyp0/
- xmobar
- xmonad config
- git
    - TODO git config
- vim
    - TODO vimrc

TODO

- ssh certs
- keepassx
- xmobar
- xscreensaver

## update alternatives?

```
sudo update-alternatives --get-selections
```
