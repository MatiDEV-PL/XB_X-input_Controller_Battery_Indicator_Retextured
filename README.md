[![License: GPL v2](https://img.shields.io/badge/License-GPLv2-blue.svg)](https://github.com/MatiDEV-PL/XB_X-input_Controller_Battery_Indicator_Retextured/blob/main/LICENSE) 
# Xbox X-input Controller Battery Indicator Retextured
A tray application that shows a battery indicator for an Xbox-ish controller and gives a notification when the battery level drops to (almost) empty. 
In retextured verison there were made changes to icons.

When more than one controller is present, the tray icon will cycle through the status display every 5 seconds.

The standard size of the taskbar:              

![Tray icon](https://i.imgur.com/0hjGORC.gif)
                                                        
In a larger size (just because, why not?):

![Tray icon](https://i.imgur.com/BqiRGXX.gif)

When a controller reaches low battery level, a notification is displayed.  

![Imgur](https://i.imgur.com/LPUBWtl.png "Toast message with low battery warning")


Controllers reported as working/being recognized so far:
* XBox Series X/S + dongle
* XBOne S + dongle 
* XBOne S + Bluetooth
* XBOne Elite + dongle
* XBOne + dongle
* XB360 

Currently known issues/limitations:
* Series X/S controllers connected via Bluetooth won't report any or a completely wrong battery level. This seems to be an issue with Microsofts BT implementation and I can't do anything about it. See Issue [#49](https://github.com/NiyaShy/XB1ControllerBatteryIndicator/issues/49) for details.
* initial recognition of a newly connected controller can take a while. It will be displayed as "waiting for battery level data" at first but should switch to battery level after ~10 seconds and a button press. (This might be a limitation of the XInput API.)

Some additional details about how it works and what it shows can be found on the [orginal developer wiki page](https://github.com/NiyaShy/XB1ControllerBatteryIndicator/wiki).  
Orginal project: [XB1ControllerBatteryIndicator](https://github.com/NiyaShy/XB1ControllerBatteryIndicator).
