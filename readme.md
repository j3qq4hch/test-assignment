# SFP module

This repository contains source documentation for Gigabit SFP module based on RTL8211FS.
This is some sort of test assignment and not a real device.
The design is not tested in hardware (though looks fine in theory).

The design was done in EagleCAD. Any version starting from 7.7 should open the design just fine. 
3D model generated using NoABS.Eagle3d tool (not released yet).

The device looks like this:

<p align = center>
<img  width = 600 src = figures/overview.png>
</p>

3d model of the device is available [here](https://j3qq4hch.github.io/test-assignment/index.html?model=sfp.glb).

Schematic in pdf format can be found [here](sch.pdf).

One of the requirements of this test assignment was to find flaws in the design and fix them. Below is a list of these flaws:

* The overall schematic quality is poor.
* TXD+/TXD- on SFP connector side must be swapped.
* Ethernet connector has no embedded magnetics. Had to replace connector with [HanRun HR911130C](https://www.chipdip.ru/product/hr911130c-razyomy-i-soediniteli-hanrun-8048835943).
* The PCB is too narrow for the ethernet connector. It has to be a bit wider. 
* Some of the decoupling capacitors missing.
* Using proprietary and very expensive software for a test assignment likely assumes that the candidate will use pirated software, which is not a good practice.