---
title: A Year with the Anet A8 3D Printer
tags: [anet, a8]
categories: [3d-printing]
---

Last year, after using 3D Hubs several times, I decided to take the jump; I'm getting myself a 3D printer.
I decided to get an Anet A8 for 2 reasons:
 
- it's cheap
- lots of upgrades available

I paid 160 EUR for the printer. It's possible to get it for a lower price as there are occasional promotion sales on sites like [Banggood.com](https://www.banggood.com/Anet-A8-3D-Printer-DIY-Kit-1_75mm-0_4mm-Support-ABS-PLA-HIPS-p-1130694.html?p=E8231110898371201705)

### Assembly
 
The assembly went quite smooth, the hardest part was removing all the protective tape from the acrylic parts.
There's just one thing to be aware of; the instructions for the installation of the H frame on the heated bed are wrong.
This has to be mounted the opposite way so the belt below is straight.

I was very impressed with the first prints. I only had to tighten the belts a bit to get a very nice 
[XYZ calibration cube](https://www.thingiverse.com/make:370493)

### Printing bed surface

The printer has some yellow tape on the hotbed. This was coming of fast after removing the first few prints from the bed.
I needed a better solution for this so I got a [215 x 215 x 3 mm glass plate](https://www.velleman.eu/products/view/?id=417314)
The glass plate causes a smooth side when printing which I think is really nice. When the bed is leveled properly it sticks
very well. In case of smaller prints with less contact to the bed I also print a raft so the print won't get loose while printing.
Please note I only print with PLA filament.

### Upgrades

The Anet A8 is a clone of Prusa i3. There are lots of modifications on thingiverse to make it look even more like a Prusa i3.
One of the nicest modifications I did was the spool holder that goes on top of the frame. This saves some space and causes
the filament to go in a straight line to the extruder. The printer could now fit on a IKEA Lack side table instead of taking up
all my desk space.

One of the things that was very time consuming with this printer was levelling the bed. Adding wing nut bed level screw knobs
and spring bushings made it a lot easier to level the bed. I had to drill out the holes on the heat bed a bit 
as these were threaded.

With the printer on the small side table it made quite some noise while printing. I printed 6 vibration dampers to reduce this noise.
Also I changed the cooling fan speed to 50% in my slicer software.

Another known problem with this printer is the hotbed connector. I noticed the hotbed was not heating up properly and saw the plastic
connector got burned on both sides. I fixed this by soldering the red and black wire directly to the hotbed. To prevent issues with this
in the future I added a cable strain relief. 

One of the last thing I installed was a [MOSFET](https://www.banggood.com/3D-Printer-Parts-General-Add-on-Heated-Bed-Power-Expansion-Module-High-Power-For-Chitu-Motherboard-p-1086965.html?p=E8231110898371201705). I've added it to move some of the current from the mainboard. Older versions of the mainboard
had different connectors which could melt if not properly connected. The hotbed is now powered through the MOSFET which removes some
stress for the main board.

Some other modifications I printed which I think are nice but not really needed;

- semi circular fan duct
- filament guide
- main board cover
- extruder button
- cooling fan cover

The list of all the upgrades I've printed: [https://www.thingiverse.com/snoek09/collections/anet-a8-upgrades](https://www.thingiverse.com/snoek09/collections/anet-a8-upgrades)
