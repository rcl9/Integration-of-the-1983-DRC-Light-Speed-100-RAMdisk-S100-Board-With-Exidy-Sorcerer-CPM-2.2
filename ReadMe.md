# Integration of the 1983-era DRC 'Light Speed 100 RAMdisk' S-100 board with the Exidy Sorcerer + CP/M 2.2

This repository provides a historical and archival overview of the 1983-era "Light Speed 100" (LS-100) 256k S-100 RAMdisk board produced by Digital Research Computers. This archive will also provides the custom BIOS source code written by the author back in July 1984 to tightly integrate this card as a virtual floppy disk drive on his Exidy Sorcerer computer running CP/M 2.2 with the [Morrow Disk Jockey 2D S-100 controller card](https://github.com/rcl9/Morrow-DJ2D-CPM-22-Recompile-From-Source). The primary reason this repository was written was because the information being provided herein was simply not available openly on the Internet. 

<div style="text-align:center">
<img src="/Images/LS100 board.jpg" alt="" style="width:70%; height:auto;">
</div>

## Overview

The LS-100 board acted as a very fast CP/M floppy disk drive with a capacity of 256K. It utilized the Intel 8203-1 Dynamic RAM refresh controller and was quite reliable.  It was also IEEE-696 compliant. All operations went through 4 I/O ports which were switch configurable. The board came with some basic 8080 assembly code to get it going under CP/M. Up to 8 boards could be configured in a S-100 system.

The board was reviewed and tested in [issue 18](http://cpmarchives.classiccmp.org/cpm/Library/Magazines/TCJ/tcj_18.pdf) of the "The Computer Journal", pages 13 through to 16.

The author purchased and built the kit in July 1984 for CDN$182.

## CBIOS for the Exidy Sorcerer and Morrow DJ2D

To properly use the board it needs to be integrated into the BIOS of a CP/M 2.2 system so that the board appears as a RAM-based floppy disk drive. That CBIOS is available [herein](<Src/Morrow%20DJ2D%20%2B%20Exidy%20Sorcerer%20CBIOS%20with%20LS-100%20support%20-%20v4.0.mac>).

## Product Manual

The author has scanned in his original [product manual](<Docs/'Light%20Speed%20100'%20256k%20disk%20simulator%20manual%20-%201983.pdf>) for reference. 

## Schematics

The main logic:

<div style="text-align:center">
<img src="/Schematics/LS-100 schematics - Page 1 of 2.jpg" alt="" style="width:70%; height:auto;">
</div>
<br>

And the 256k (4 x 64k) RAM banks:

<div style="text-align:center">
<img src="/Schematics/LS-100 schematics - Page 2 of 2.jpg" alt="" style="width:70%; height:auto;">
</div>
<br>
