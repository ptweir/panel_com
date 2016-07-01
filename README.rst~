panel_com
=============
panel_com provides a serial port interface to Michael Reiser's Panel controller
 
Installation
-------------------
* Installation instructions can be found in the INSTALL file.
* Alternatively, simply copy the panel_com directory into your project.

Troubleshooting
-------------------
* Different generations of controllers expect different baudrates. Common values are 115200 and 921600. The default can be set in line 34 of panel_com.py
* If you get an error when trying to connect:
    1. Check to see if the controller shows up as /dev/ttyUSB0 (or ttyUSB1, 2, etc.)  device. Run ``ls -l /dev | grep ttyUSB`` before and after plugging in the controller USB. A new /dev/ttyUSB device should appear.
    2. If the /dev/ttyUSB device does show up, but you cannot open a connection -- e.g. you get permission denied -- then you probably need to add yourself to the correct group, usually "dialout". You can double check this by running ``ls -l /dev/ttyUSBN`` where /dev/ttyUSBN is your device.  The result should look something like this

    ``crw-rw---- 1 root dialout 188, 0 May 19 12:12 /dev/ttyUSB0``

    where whatever is in the place of "dialout" is the group for the device. You can add yourself to this group by editing /etc/group file - just put your username after the group name (there are lots of examples in the file itself). You must logout before your changes take effect.


Examples
-------------------
* Examples demonstrating how to use panel_comm can be found in the panel_comm/examples directory. 
     
Author
-------------------
* Will Dickson
* Adapted from the Panel_com class of Seth budick in PControl.
* Maintained by Peter Weir. 
