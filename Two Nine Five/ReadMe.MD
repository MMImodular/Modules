# Two Nine Five

**I am temporarily removing gerbers and .brd file while I figure out automated assembly. I will keep the schematic up and create build files to assist DIYers in the mean time.**

* Eurorack adaptation of the Buchla Model 295 10-channel comb filter
* 10 LED sliders control the amplitude of each band sent through the SUM output
* Individual channel outputs to the right of each slider
* Tunable band frequencies, Q's, and amplitude via trim pots on the back of the module.

This recreation of the Model 295 has been in my head since before I owned any modular. After using a restored Buchla at the Oberlin Conservatory of Music, the 295 became one of my favorite modules in the whole case. Buchla modular is far out of my budget so with the original schematics in hand, I made a much more compact 3U version of it. The circuitry is exactly the same, though more modern op-amps have to be used since the ones used in the original design are no longer available.

**Things to note when building**

It is absolutely imperative that you solder R13, R39, R17, R37, R19, R35, R25, and R33 properly before mounting the trim pots as they will be very difficult to reach once all components are in place. To confirm they are soldered properly, measure the resistance between the two middle pins of each trim pot location. For instance, the resistance between the middle pin of VR10 and VR9 should be roughly 68 kOhms.

In addition, please heed the warning on the front of the PCB and place the trim pots on the back of the module. There is not enough space between the PCB and panel for the trim pots and having them on the back allows for you to tune everything without taking the panel off. I kept the silk screen for the pots on the top side in order to avoid cluttering the bottom silkscreen layer.

As for the illuminated slide pots, there's a few things to consider. They are acting as cross faders so any value between 10k and 100k should work just fine. They are taking an audio signal so ideally you want audio response, but linear response will function just fine. Ideal shaft length is 15mm but I have used 10mm successfully, the tops are just a tad close to the panel. You do not want a center detent if you can help it. The sliders I used can be found on Mouser: 652-PTL20-10R0-103B2

**How to tune your 295**

* Using a VU meter, set a sine wave out to -6.5dB
* Input that sine wave to the 295 filter
* Set the frequency of the wave to match the frequency of the band you'd like to tune (e.g. 3000 Hz)
* Slide the potentiometer of the band you want to tune all the way to the right
* Turn the 20k trim pot until the SUM output of the 295 filter is at 0 dB
* Then scan your sine wave around your desired frequency and note where the VU meter peaks
* Adjust 100k trim pot until the peak happens as close to the desired frequency as possible
* Adjust the 20k trim pot a second time so the output is back at 0db as the 100k trim pot has an effect on amplitude.
* Repeat for each band

PCB and panel designed by me

Original schematic by Don Buchla

![Imgur](https://i.imgur.com/43DXM32.jpg)

![Imgur](https://i.imgur.com/BFru6uz.jpg)
