# battery-monitor
Minimalistic battery monitor for GNU/Linux laptop

# Purpose
Show battery icon in system tray; hover over icon for remaining battery percentage and time

# What you need
0. GNU/Linux operating system and this script
1. Suitable icons (provided)
2. Suitable low battery, a/c connected, a/c disconnected sounds (provided)
3. **mktrayicon** utility somewhere in your PATH (x86_64 binary provided; source code [here](https://github.com/jonhoo/mktrayicon))
4. mktrayicon needs **gtk3** and any panel with a system tray
5. **aplay** utility (usually part of *alsa-utils* package)
6. Check "user variables" at top of script for correctness

# Installation
```
$ sudo apt install alsa-utils libgtk-3-0
$ cd /tmp
$ wget https://github.com/bdantas/battery-monitor/archive/master.zip
$ unzip master.zip
$ cd battery-monitor-master
$ sudo cp battery-monitor mktrayicon /usr/local/bin # the provided mktrayicon binary is for x86_64
$ sudo chmod a+x /usr/local/bin/battery-monitor /usr/local/bin/mktrayicon
$ sudo mkdir -p /usr/share/icons/battery-monitor
$ sudo cp *.png /usr/share/icons/battery-monitor
$ sudo mkdir -p /usr/share/sounds/battery-monitor
$ sudo cp *.wav /usr/share/sounds/battery-monitor
```
Note: If your operating system is not Debian-like, adjust the first step

# Usage
Run `battery-monitor &` at boot
