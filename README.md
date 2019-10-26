# battery-monitor
Minimalistic battery monitor for GNU/Linux laptop

# Purpose
To show a battery icon in the system tray; hovering over the icon shows remaining battery charge both as percentage and as time remaining

# Usage
Run `battery-monitor &` at boot

# What you need
0. GNU/Linux operating system and this script
1. Suitable icons (provided)
2. Suitable low battery alert sound (provided)
3. `mktrayicon` utility somewhere in your PATH (x86_64 binary provided; for other architectures you'll need to compile from [source](https://github.com/jonhoo/mktrayicon))
4. Check "user variables" at top of script for correctness
