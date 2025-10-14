# Pomodoro plugin for an Xfce4 Panel

This bash script uses xfce4-genmon-plugin, zenity and libnotify to create a simple Pomodoro timer in an Xfce4 Panel.
After xfce4-genmon-plugin is added to the Panel it should be configured to point to the pomodoro.sh script.  

The icons are from https://github.com/mozilla/fxemoji

## Installation Instructions:
1. Download pomodoro.sh or clone the repository
1. Install xfce4-genmon-plugin: `# apt-get install xfce4-genmon-plugin`
1. Right click on your Xfce Panel, go to **Panel** => **Add New Items...**
1. Search for **Generic Monitor**, and select it.
1. Right click on the newly added monitor in the Panel, and select **Properties**
1. In the new window enter the path to `pomodoro.sh` in the *Command* field. Pass optional arguments here.
1. Uncheck *Label*
1. Set a period of **1** seconds. This is the refresh/recheck period.
1. Click on your new panel item to start the timer.
1. Stop procrastinating and start working :)

## Available Command Line arguments:
| Option                       | Description                       |
| ---------------------------- | --------------------------------- |
| `-n, --click`                | start or stop the timer |
| `--pomodoro <minutes>`       | minutes for the pomodoro cycle (default: 25) |
| `--short-break <minutes>`    | minutes for the short break cycle (default: 5) |
| `--long-break <minutes>`     | minutes for the long break cycle (default: 15) |
| `--cycles <number>`          | number of pomodoro cycles before long break (default: 4) |
| `--disable-sound`            | disable the sound notification when a pomodoro cycle completes |
| `--icon-size <number>`       | change the size of the toolbar icon (default: 24, available: 16, 24, 32) |
| `-h, --help`                 | display the help |