# XBox One Controller Battery Indicator
A tray application that shows a battery indicator for an Xbox-ish controller and gives a notification when the battery level drops to (almost) empty. 

It was originally written for the XBox One controller since Microsoft dropped all visual hints for low battery, but it should work with any gamepad that can be addressed via XInput (which should be all controllers that work in XBox-controller-enabled games).

**Download link for a "ready to run" version at the bottom of this page(or under "Releases" in the side bar)!**  
(The green download button at the top is for the source code package)

When more than one controller is present, the tray icon will cycle through the status display every 5 seconds.

![Tray icon](https://i.imgur.com/rxWAsu8.gif "Tray icon cycling through multiple controllers")

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

**[You can download the latest version here](https://github.com/NiyaShy/XB1ControllerBatteryIndicator/releases).**  
Some additional details about how it works and what it shows can be found on the [wiki page](https://github.com/NiyaShy/XB1ControllerBatteryIndicator/wiki).  
Found a bug or wanna give feedback? Open an issue here in github or leave a comment over on [reddit](https://www.reddit.com/r/xb1cbi).