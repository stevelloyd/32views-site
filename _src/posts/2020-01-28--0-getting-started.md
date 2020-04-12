    Title: (0---Getting started)
    Date: 2020-01-28T20:15:55
    Tags: chapters, DRAFT

## Getting started...setting up your Pi and installing Racket

This first chapter will get us to the stage of having a Pi, running Racket and having a look at what a program lookd like in Racket.
<!-- more -->

### Items to obtain

You'll need to buy or borrow:

* Pi, case and power supply
* monitor
* an SD card with the latest Raspbian release

### Which model of Pi?

Currently the latest Pi is the 4 model B availabile with 1/2/4GB of RAM. Ideally, the 2 or 4GB model of this is perfect for these projects. Alternatively the earlier 3 B+. The Pi Zero models *can* run Racket, but are best suited when you come to embed some intelligence in a finished project rather than for learning and development. 

For a Pi 4 model B, it's worth also adding a heatsink for the processor; but bear in mind that we want to wire up our Pi to the external world so heatsink cases which restrict access to the GPIO[^GPIO] aren't so useful.

### Cases

As there will be lots of 

[^GPIO]: The set of pins which allow connecting your Pi to the outside world.




```Racket
(+ 2 2)
⇒ 4

(define (+2 n)
(+ 2 n))
```


