MCPiLight
=========
This program requires the [ComputerCraft](http://www.computercraft.info/) mod for [Minecraft](https://minecraft.net/).

These programs work to together to make an LED connected to the [Raspberry Pi](http://www.raspberrypi.org/) when a lever is switched in Minecraft.
The LED can connect to any free GPIO pin on the Pi. It is connected to pin 23 in my example

The python file runs on the Raspberry Pi. You will have to run it as root: `sudo python LED.py`

The other file goes on the computer in Minecraft. You can either move it into the proper directory in your Minecraft saves folder. The command line parameters for the startup program are: `startup [raspberry pi url] [side] [delay]`. The raspberry pi url has to have `http://` at the beginning and the port `:3141` at the end. Delay is how long to wait between polls. It is recommended to have at least a one second delay. The default values are `http://raspberrypi.local:3141`, `top` and `1`.

This program is not just limited to LEDs and levers. It could be expanded to control nearly anything connected to the Pi using a variety of items in Minecraft.
