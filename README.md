# GPI-GPIO-action
Volumio plugin
The plugin can be used on the Volumio player, when installen on RaspberryPi.
The function is to be able to control the player, using real hardware push buttons.
You can use any of the free GPIO, to activate controls of the volumio player, like
play, stop, pause, mute, unmute, toggle mute/unmute, toggle play/stop, volume up, volume down, shutdown.
You can also use the buttons to select and play webradiostations, from your webradio favorites.
The user interface contains a "settings", in the "Plugin" subsystem, where it is possible to assign GPIO numbers to buttons, and to tell what the action should be.
My player is on a Raspberry Pi B+, with a IQaudio Pi-DigiAMP+, 
and I use a plug with 2x6 pins placed on RPI pin 7-18
Pin 9 on the RPI connector is ground, and is connected to pin1 of all my hardware buttons.
Pin 7 on the RPI connector is GPIO4, and is connected to pin2 of one of my buttons.
In short form the connections is:
RIP pin -> button number - button pin number ( GPIO number )
7 -> 1 pin2 ( GPIO4 )
8 -> 2 pin 2 ( GPIO14 )
9 -> 1,2,3,4,5,6,7 pin 1 ( ground / 0Volt )
10 -> 3 pin 2 ( GPIO15 )
11 -> 4 pin 2 ( GPIO17 )
12 -> 5 pin 2 ( GPIO18 )
13 -> 6 pin 2 ( GPIO27 )
14 no connection
15 no connection is used as HW mute on Pi-DigiAMP+, but could also be used to any other function.
16 -> 7 pin 2 ( GPIO23 )
17 + 3,3 Volt from RPI. Used to pull up resistors.
18 -> 8 pin2 ( GPIO 24 )

