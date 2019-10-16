# battery-monitor
Minimalistic battery monitor for GNU/Linux laptop

# Purpose
Simple shell script for GNU/Linux that runs in the background, showing remaining battery charge (as a percentage) on the desktop. Hovering over the percentage shows battery time left (in hours:minutes).

# Usage
Run `$ battery-monitor &` at boot or at any other time to launch the script

The only adaptations you need to make (to the top of the script) are:
1. Choose the x and y coordinates of where the percentage should appear on the screen
2. Choose background color of the applet 
3. Make sure the `sys` and `proc` directories are correct

# Dependencies
- GNU/Linux OS
- **dzen2**
