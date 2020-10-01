# battery-monitor
Minimalistic battery monitor for GNU/Linux laptop

# Purpose
Show battery icon in system tray; hover over icon for remaining battery percentage and time

# What you need
0. GNU/Linux operating system and this script
1. Suitable icons (provided)
2. Suitable low battery, a/c connected, a/c disconnected sounds (provided)
3. **mktrayicon** (x86_64 binary provided; source code [here](https://github.com/jonhoo/mktrayicon)) or **yad**
4. **gtk3**
5. any panel with a system tray
6. **aplay** utility (usually part of *alsa-utils* package)
7. Check "user variables" at top of script for correctness

# Example installation
```
$ sudo apt install yad libgtk-3-0 alsa-utils
$ cd /tmp
$ wget https://github.com/bdantas/battery-monitor/archive/master.zip
$ unzip master.zip
$ cd battery-monitor-master
$ sudo cp battery-monitor /usr/local/bin/
$ sudo chmod a+x /usr/local/bin/battery-monitor
$ sudo mkdir -p /usr/local/share/icons/battery-monitor
$ sudo cp *.png /usr/local/share/icons/battery-monitor/
$ sudo mkdir -p /usr/local/share/sounds/battery-monitor
$ sudo cp *.wav /usr/local/share/sounds/battery-monitor/
```
Note: If your operating system is not Debian-like, adjust the first step

# Usage
Run `battery-monitor &` at boot
