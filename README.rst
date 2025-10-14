Pomodoro plugin for Xfce4 panel
===============================

This bash script uses xfce4-genmon-plugin, zenity and libnotify to create a simple Pomodoro timer in an Xfce4 panel.
After xfce4-genmon-plugin is added to the panel it should be configured to point to the pomodoro.sh script.  

The icons are from https://github.com/mozilla/fxemoji

Instructions for the Xfce Desktop Environment:
------------------------------------------------------------------
#. Download pomodoro.sh or clone repository
#. Install xfce4-genmon-plugin: ``# apt-get install xfce4-genmon-plugin``
#. Right click on your XFCE panel, go to **Panel** => **Add New Items...**
#. Search for **Generic Monitor**, and select it
#. Right click on newly added monitor in panel, and select **Properties**
#. In new window enter path to ``pomodoro.sh`` in *Command* field. Pass optional arguments here.
#. Uncheck *Label*
#. Set a period of ``1`` seconds. This is the refresh/recheck period.
#. Set font large enough to see remaining time clearly.
#. Click on your new panel item to start the timer.
#. Stop procrastinating and start working :)

Available Command Line arguments:
------------------------------------------------------------------
  
| Option | Description |
| --- | --- |
| -n, --click                | start or stop the timer |
| --pomodoro <minutes>       | minutes for the pomodoro cycle (default: 25) |
| --short-break <minutes>    | minutes for the short break cycle (default: 5) |
| --long-break <minutes>     | minutes for the long break cycle (default: 15) |
| --cycles <number>          | number of pomodoro cycles before long break (default: 4) |
| --disable-sound            | disable the sound notification when a pomodoro cycle completes |
| --icon-size <number>       | change the size of the toolbar icon (default: 24, available: 16, 24, 32) |
| -h, --help                 | display the help |
