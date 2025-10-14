Pomodoro plugin for Xfce4 panel
===============================

This bash script uses xfce4-genmon-plugin and libnotify to create a simple Pomodoro timer for Xfce4 panel.
After xfce4-genmon-plugin is added to the panel - it should point to the pomodoro.sh script.  

To disable sound notifications, pass the `--disable-sound`` flag in the Generic Monitor command.  

To configure hard-coded parameters please go to pomodoro.sh and configure:  
  size - Icon size in pixels  
  pomodoro_time - Time for the pomodoro cycle (in minutes)  
  short_break_time - Time for the short break cycle (in minutes)  
  long_break_time - Time for the long break cycle (in minutes)  
  cycles_between_long_breaks - How many cycles should we do before long break  
  notify_time - Time for notifcation to hang (in seconds)  

The icons are from https://github.com/mozilla/fxemoji

Instructions for XUbuntu (and probably other XFCE from the family)
------------------------------------------------------------------
#. Download pomodoro.sh or clone repository
#. Install xfce4-genmon-plugin: ``# apt-get install xfce4-genmon-plugin``
#. Right click on your XFCE panel, go to **Panel** => **Add New Items...**
#. Search for **Generic Monitor**, and select it
#. Right click on newly added monitor in panel, and select **Properties**
#. In new window enter path to ``pomodoro.sh`` to *Command* field
#. Uncheck *Label*
#. Set a period of `1` seconds. This is the refresh/recheck period.
#. Set font large enough to see remaining time clearly.
#. Click on your new panel item to start the timer.
#. Stop procrastinating and start working :)


Happy Pomodoro !!
