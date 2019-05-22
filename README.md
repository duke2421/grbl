![GitHub Logo](https://github.com/gnea/gnea-Media/blob/master/Grbl%20Logo/Grbl%20Logo%20250px.png?raw=true)

Added Support for a new Arduino-Nano-Shield designed by Till Nenz. You can find more information about his shield here on Github.
Link to Tills repo: https://github.com/tnn85/MPCNC-Nano-Estlcam-Shield

With GRBL you can use a Laser module easily with LaserGRBL or with Laserweb4. With Estlcam the Laser works not very well, so I decided to make a fork of the GRBL-Code, so that it can be used with Tills shield. If you not have this shield, use the [original GRBL code.](https://github.com/gnea/grbl)   

Due to significant pin changes some functions of GRBL can not be used with the shield fom Till, so I removed the whole code for:

RESET      
FEED_HOLD     
CYCLE_START  
SAFETY_DOOR

These four functions are without function and Terminals E7 and E8 are not useable.
### You must not connect anything to these Pins!

The endstops at X, Y and Z are tested and working. Connect X Endstop to E1, Y Endstop to E2 and Z to E3. The Probe should be connected to E4, but this is not tested yet.


-------------
Removed all lines of the original Readme, you can read it at the [original repo](https://github.com/gnea/grbl).
Because I haven't done anything big to the code, the Donate button will stay as it is an always point to gneas repo.

-------------
Grbl is an open-source project and fueled by the free-time of our intrepid administrators and altruistic users. If you'd like to donate, all proceeds will be used to help fund supporting hardware and testing equipment. Thank you!

[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CUGXJHXA36BYW)
