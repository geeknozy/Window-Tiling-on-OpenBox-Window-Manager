# Window Tiling on OpenBox Window Manager
The following is the xml code to get the window tiling feature on OpenBox Window manager

#Verticle Tiling
![alt text](https://raw.githubusercontent.com/geeknozy/OpenBox-Window-Tiling-.rc-file/main/verticle_tile.jpg)

#Horizontal Tiling
![alt text](https://raw.githubusercontent.com/geeknozy/OpenBox-Window-Tiling-.rc-file/main/horizontal_tile.jpg)


OpenBox Window manager is highly configurable window manager that can be used on *NIX Operating systems that has capability of replacing an entire desktop environment.

OpenBox by default is a floating window manager, and have no tiling feature keybinding enabled by default and has the .rc file written and can be edited using xml.

Follow along this steps to get the tiling window feature.

Step 1 : Open your favourite terminal and type 

```
cd /home/yourusername/.config/openbox
```

Step 2: list all the files

```
ls -a
```

Step 3: Open rc.xml (on vanilla OpenBox Session) or lxqt-rc.xml file on LXQT Desktop Environment with OpenBox Window Manager.

for openbox type below command
```
sudo nano rc.xml
```

for lxqt with openbox type 
```
sudo nano lxqt-rc.xml
```

Step 4: Find the <keyboard> section and go to the end of ```<keyboard>``` ie: ```</keyboard>``` section.

Step 5: Just above </keyboard> paste my configuration code given above.

Step 6: Save and exit the .xml file

Step 7: Type the following command for changes to take place on the terminal.

```
openbox --reconfigure
```

Key Bindings are as follows

1. Left half tiling vertically <br/>
```CTRL + WINDOWS_KEY + LEFT_ARROW``` <br/>

2. Right half tiling vertically <br/>
```CTRL + WINDOWS_KEY + RIGHT_ARROW``` <br/>

3. Bottom half tiling horizontally <br/>
```CTRL + WINDOWS_KEY + BOTTOM_ARROW``` <br/>

4. Upper half tiling horizontally <br/>
```CTRL + WINDOWS_KEY + UPPER_ARROW``` <br/>

NOTE: If you are using keybindings that are already in use you may encounter errors change the xml code accordingly.
