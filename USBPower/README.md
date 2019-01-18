# USB Power

* Based on Tom Whitwell's StupidUSBPower
* Integrated better DC-DC converter and removed frivolous features
* Rated to 416mA, capable of 110 ~ 140% overload with automatic recovery once fault condition is removed

This power supply is a low cost and low profile way to power a small lunchbox eurorack system. It is also a useful power supply for testing newly built modules outside of a larger system, especially if you must commute to your workspace.

___

The Meanwell DC-DC converter used in this power supply has a few important specifications to consider.
* Under full load, the DC-DC converter will draw upwards of 2300mA direct from your USB power brick. Make sure it can supply ~3A if you plan on running your PSU near the max current spec.
* Maximum load capacitance is 440uF per output. Approaching this may cause instability upon power-up. This needs more investigation on my part so I will update this list if I figure out more specific cases of instability.
* There is an under-voltage lockout implemented in this converter. It takes 4.4V to start the converter and it will shut down if it goes below 4.2V. This important because some users have experienced instability with USB cables that are incapable of supplying power. Voltage drop across the cable may be enough to go below 4.2V and result in a boot loop.

___
**Known module incompatibilities**

These are modules that people have plugged in and run in to boot looping issues with, despite the PSU operating normally otherwise. I do not have the ability to test each and every module that comes up, but if you own any of these I encourage testing it for yourself and sending me a message or email detailing what you found.

* Synthrotek 308 Distortion
* Jomox ModBase 09
* Strymon Magneto (works solo, but loops if other modules are present)

___
**Where to buy PCBs** 

* [Modular Addict](https://modularaddict.com/mmi-usbpower-pcb)

* [Pusherman](https://pushermanproductions.com/product/mmi-modular-usb-power-supply/) (this is the best spot to pick one up if you live outside the USA)

* [Directly from me!](https://reverb.com/item/13361422-mmi-modular-eurorack-usb-power-supply-pcb-only)


![](https://modularaddict.com/media/catalog/product/cache/1/image/1100x1100/9df78eab33525d08d6e5fb8d27136e95/m/a/max-usbpow-pcb.jpg)
