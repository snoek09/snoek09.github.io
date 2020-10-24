---
title: Anet A8 - AM8 Aluminium Frame Build
hero: /images/am8-build/am8-build.jpg
date_lastmod: 2019-10-13
---

The acrylic frame that came with my Anet A8 is not the most solid construction.
Adding a [spool holder on top](/blog/2018/05/06/a-year-with-the-anet-a8-3d-printer/) of it doesn't make things better.

One of the bigger upgrades I could do is the AM8 metal frame build.
This upgrade will make a sturdy frame while re-using as many components as possible.
<!-- more -->

### Parts needed

- [Reinforced AM8 frame parts](https://www.thingiverse.com/thing:2657605)
- [Other AM8 frame parts](https://www.thingiverse.com/thing:2263216)
- [Aluminium 20x20 profile and corners set](https://www.dold-mechatronik.de/AM8-Aluprofile-und-12-Winkel-20x20)

Check the [BOM](https://cdn.thingiverse.com/assets/a3/bd/fb/22/18/BOM.pdf) for screws, nuts and other materials you might need.

For connecting bolts to the extrusion I used M5 T nuts.

### Missing Z-axis corner bracket

The 2020 aluprofile set from dold-mechatronik is convenient though be aware the the corner brackets won't fit on the Z-axis connection.
For this I printed a few [Z corner brackets](https://www.thingiverse.com/thing:3140856).

### Bowden extruder parts

A while ago I have changed the standard extruder with a bowden extruder. I find it a lot easier to change the filament this way.
Luckily there's also a [bowden extruder mount for the AM8](https://www.thingiverse.com/thing:2383009). It re-uses most parts of the original extruder.
Only the [extruder button](https://www.thingiverse.com/thing:2501601) is 3D printed.

### Optional parts

I didn't print the case for the LCD as I don't need it; I'm using a Raspberry Pi with [OctoPrint](https://octoprint.org/) and [Printoid](https://printoid.net/).
This way I can control and monitor prints from my smartphone. I can even watch the print in progress as the Pi Zero has a camera attached to it.

**Update:** it's not recommended to use a Raspberry Pi Zero W with OctoPrint. Severe performance issues were observed, caused by the WiFi interface when bandwidth is utilized (e.g. the webcam is streamed), negatively impacting printing quality. More info in [this github issue](https://github.com/guysoft/OctoPi/issues/318#issuecomment-284762963).

Some other parts that have been upgraded/added during this build;

- Z-axis couplers; plum shaft
- mainboard: Anet A8 board version 1.7; added fuse and 24 volt support
- 12v to 5v step down converter; power Pi Zero from power supply
- 8mm braided cable sleeve

All 3d printed parts are listed in a [AM8 Thingiverse collection](https://www.thingiverse.com/snoek09/collections/am8).

![Anet A8 - AM8 build](/images/am8-build/am8-build.jpg){.img-fluid}

