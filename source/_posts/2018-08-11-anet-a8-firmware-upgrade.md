---
title: Upgrading the Anet A8 firmware to Marlin 1.1.x
tags: [anet, a8]
categories: [3d-printing]
---

The firmware of the Anet A8 3D printer is based on Marlin. This is an outdated version though.
One of the most important features it's missing, is a security check on the heating elements.
In my post about [Anet A8 upgrades](blog/2018/05/06/a-year-with-the-anet-a8-3d-printer) you can
read what can happen to the heat bed connector.

<!-- more -->
With this upgrade the Anet A8 will be safer to use. It will stop heating the heat bed and extruder element
after it reaches a certain temperature. Also if you want to use auto-levelling of the heat bed using a sensor
you need to upgrade to Marlin. This also requires some small changes to the Marlin code which will not be discussed here.

### What you need

- [Arduino IDE software](https://www.arduino.cc/en/Main/Software)
- [Anet A8 board definition for Arduino](https://github.com/SkyNet3D/anet-board)
- [Marlin firmware](https://github.com/MarlinFirmware/Marlin/archive/1.1.x.zip)

Instructions and screenshots below are from Ubuntu Linux.
Depending on your operating system the location of the Arduino files will be slightly different.

### Move Anet A8 board definition files

The board definition files enable the Arduino IDE to compile firmware (in this case Marlin) for Anet 3D printers.

Copy the anet folder to the Aruindo\hardware folder. Create the hardware folder if it doesn't exist.

![Anet A8 board defination files](/images/marlin/board-definition-files.png){.img-responsive}

### Copy Marlin example configuration 

Unzip the Marlin firmware and go to the Marlin\example-configurations\Anet\A8 folder:

![Marlin A8 configuration files source](/images/marlin/marlin-a8-configuration-source.png){.img-responsive}

Copy the 2 configuration files to the Marlin folder:

![Marlin A8 configuration files destination](/images/marlin/marlin-a8-configuration-destination.png){.img-responsive}

Open the Marlin.ino file in Arduino IDE:

![Arduino IDE - Open Marlin.ino](/images/marlin/arduino-ide-open-marlin-ino.png){.img-responsive}

Connect your printer to your computer using USB.
Make sure that Anet V1.0 is selected as Board:

![Arduino IDE - Select Anet Board](/images/marlin/arduino-ide-select-board.png){.img-responsive}

Port should be set to USB:

![Arduino IDE - Select USB Port](/images/marlin/arduino-ide-select-port.png){.img-responsive}

Upload the firmware by clicking the upload button:

![Arduino IDE - Upload button](/images/marlin/arduino-ide-upload.png){.img-responsive}

When the update is done the printer will restart and your printer menu will look like this:

![Updated printer menu](/images/marlin/updated-menu.jpg){.img-responsive}

