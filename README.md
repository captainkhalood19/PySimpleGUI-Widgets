# PySimpleGUI-Widgets
Rainmeter-like Widgets for your desktop using the easy to use PySimpleGUI package

You will need to install PySimpleGUI for any of these widgets to execute.

## List of Widgets

--------

NOTE - The COVID19 Widget has been removed.  The data sources were changed and it no longer properly worked. Sorry about that!

--------------------

## System Status Dashboard

Displays some stats found via the psutil package (required)

![System Status Dashboard](https://user-images.githubusercontent.com/46163555/83331138-38b37080-a262-11ea-83a6-3864f7b8291e.gif)

This is one of the older programs.  Hopefully the coding conventions are up to date.

It uses a class to define the individual graphs which is likely a great way to have done it.  It's worth a look to see if it gives you some ideas.  Only recently re-discovered.

---------------------


## Weather - Current Weather Conditions

You will need to obtain an API key (APPID) from https://home.openweathermap.org/ in order to run this Widget.

Change the colors to any of the PySimpleGUI Themes.

Your key and location are saved in a config file (.CFG).  Any time you change the key or the location it will be saved in your config file.

![SNAG-0649](https://user-images.githubusercontent.com/46163555/76476971-3ddaef00-63da-11ea-8e7e-3aafb1485185.jpg)


-------------------------

## CPU Core Usage

This one uses psutil to graph the CPU time used by each of your CPU's cores.

![PSG CPU Cores Scrolling](https://user-images.githubusercontent.com/46163555/72114378-52830400-3311-11ea-8584-32bde5c265db.gif)

--------------------------

## Disk Drive Usage

Another one based on psutil.  The Windows version works well, however the partition stats returned on Linux don't have values populated to determine the stats.  Maybe it works differently on Linux?  They come out to all 0's on Linux (sorry Linux users)

Changing the theme will instantly give you a different text and background color, but it is not what is used to determine the bar colors.  Those are created from a simple list of colors defined at the top.  It's the same color combination used in the CPU core usage, so those 2 widgets match.  Feel free to replace with your own color scheme.

Standard black color theme


![image](https://user-images.githubusercontent.com/46163555/84708140-efd00d00-af2d-11ea-890d-cc1c40fbca46.png)

A dark green

![SNAG-0831](https://user-images.githubusercontent.com/46163555/84706443-f14c0600-af2a-11ea-98a5-086aad83286f.jpg)

A light green

![SNAG-0830](https://user-images.githubusercontent.com/46163555/84706444-f1e49c80-af2a-11ea-9d1e-145471853700.jpg)

One of the grays

![SNAG-0829](https://user-images.githubusercontent.com/46163555/84706445-f1e49c80-af2a-11ea-8b9e-f76256180941.jpg)

The default alpha value is .7 which is why these images' colors are muted.  This is what no transparency (alpha 1.0) with a black theme looks like:

![image](https://user-images.githubusercontent.com/46163555/84708226-1c842480-af2e-11ea-80f8-c58ffec667b3.png)


To exit click the "X" at the bottom.  Kept the interface super minimal by not using buttons, but instead simple clickable Text.

Copyright 2020 PySimpleGUI.org