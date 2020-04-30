    Title: (0---Getting started)
    Date: 2020-04-26T12:03:00
    Tags: chapters, DRAFT

## Getting started...setting up your Pi and installing Racket

This first chapter will get us to the stage of having a Pi, running Racket and having a look at what a program looks like in Racket.  
<!-- more -->

The best resource on setting up a Pi system is, understandably on the [Raspberry Pi website](https://projects.raspberrypi.org/en/projects/raspberry-pi-setting-up), so refer to this after scanning the following info.

### Items to obtain

You'll need to buy or borrow:

* Raspberry Pi 
* case (not essential but handy to protect the Pi)
* power supply
* monitor or TV with a cable to connect to the Pi
* keyboard and mouse
* an SD card with the latest Raspbian release

The dynamic market in Pi accessories mean that there are a multitude of manufacturers of the components needed, and multiple stockists of particular models.

### Which model of Pi?

Currently the latest Pi is the 4 model B availabile with 2 or 4GB of RAM. Either of these is perfect for these projects. Alternatively the earlier 3 B+ model is fine, with a loss in speed over the new model. The Pi Zero or earlier models *can* run Racket, but are best suited when you come to embed some intelligence in a finished project rather than for learning and development. 

For a Pi 4 model B, it's worth also adding a heatsink for the processor; but bear in mind that we want to wire up our Pi to the external world so heatsink cases which restrict access to the GPIO[^GPIO] aren't so useful.

### Cases

As there will be lots of connecting and disconnecting wires and boards to the Pi in this project, cases which allow easy access are most useful. So, the case below doesn't completely enclose the Pi, and the 40 GPIO pins at the top have access. The heatsink has its height tailored to allowing boards (HATs)[^HAT] to be added to the top of the Pi without risk of mechanical fit problems.


![A Raspberry Pi in case](/img/ch00/ch00-01-o.jpeg)

### Power supply

For a P4 this is a 5 volt / 3 amp supply with a USB-C connector. For Pi 3, 2 amps and a micro USB connector.

### Monitor

A monitor with an HDMI input is ideal (or TV if you can pry it away from others). For options see the Raspberry Pi site link above.

### Keyboard and mouse

You'll need a wired (USB) keyboard and mouse to setup and use the Pi. A 'with a dongle' type wireless keyboard/mouse is also fine. While Bluetooth keyboards/mice are usable once you've set up the Pi, they're not for the initial setup process.

### SD card with Raspbian

The Raspberry Pi setup page talks through the creation of an SD card (pick a 16GB one if you can to give plenty of spare space). To avoid distractions you're better off downloading the *Raspbian Buster with Desktop* option. You can always swap out this SD card for the full version if you want to try other options.

[^GPIO]: The set of pins which allow connecting your Pi to the outside world.

[^HAT]: Boards (**H**ardware **A**ttached on **T**op) which can be attached to the Pi to provide extra facilities---displays, sensors etc.



```Racket
(+ 2 2)
⇒ 4

(define (+2 n)
(+ 2 n))
```


