# OFOF1
Open-frame case design for the Open Frame1 board


## Overview

The goal of this project is to create a "bare miniumum" case design for the OF1 board, allowing aspiring makers to construct quality digital controllers as cheaply and simply as possible.

The controller is built as three layers (bottom panel, OF1 board, top panel) separated by standoffs leaving the sides open, hence the "open frame" in the title.  There are two versions of the OFOF1 case, as shown below.  The first one (labeled OFOF1 in the files) uses a top panel with circular cutouts for 3D printed MX switch button housings.  The second version (OFOF1_alt) uses a top panel with square cutouts that fit the MX switches directly.

![image](https://user-images.githubusercontent.com/95242582/177418564-77c9fb9a-2c2d-4ff1-bf36-832a5984891e.png)

![image](https://user-images.githubusercontent.com/95242582/177419836-ed6ed355-e087-4fd6-98e2-bb088412e568.png)

## OF1 Board

Please refer to the Open Frame1 repository for information about the board

https://github.com/GregTurbo/Open-Frame1

## Panels

There are many ways to fabricate the top and bottom panels.  The method I am using is ordering them as aluminum PCBs from JLCPCB.  This is cheap, strong, and allows for logos or other designs to be built into the panel.  
![image](https://user-images.githubusercontent.com/95242582/177420697-fc26cb6a-f005-4b2a-90ea-1a2d32045680.png)
However, JLCPCB has a minimum order quantity of 5, so this is not the most economical for a one-off build.

Another good method would be to order the panels through a laser-cutting service like SendCutSend (for those in the USA/Canada).  3mm acrylic or 1.6mm aluminum would both be suitable materials, and wouldn't be very expensive to make.  The panels can also be cut by hand from MDF or plywood or whatever.  Just know that you may need longer screws if you use a material thicker than 3mm.

Important note: assuming you have long enough screws, the bottom panel can be as thick as you'd like.  The top panel however should be 3mm or less in thickness to allow the screw-together button housings to fit properly.  For the OFOF1_alt, the top panel should be 1.5-1.6mm thick to allow the switches to clip into place.

The files for the bottom panel, top panel, and alternate top panel are provided in DXF format (2D CAD), STEP format (3D CAD), and as Gerber PCB fabrication files.  

Outer dimensions of the panels are 14.5"x7".


## Standoffs

The standoffs that hold the layers at the proper spacing are designed to be 3D printed.  They can be printed at home or ordered using an online 3D printing service such as the one offered by JLCPCB.  If ordering from JLC, it is fine to use the cheapest option for resin (9000R), and make sure to use the versions of the files with x8 or x10 in the filename. 

![image](https://user-images.githubusercontent.com/95242582/177422742-10cc2180-853b-4335-b5df-835c6af1c75a.png)


A complete build requires 4 corner standoffs, 5 bottom standoffs, and 5 top standoffs.  Note that there are different versions of the corner and top standoffs for the OFOF1_alt build configuration (tall ones are for OFOF1, short ones are for OFOF1_alt).

Files for these are provided in STL format, both as individual parts for at-home printing and panelized parts for ordering.  

## Buttons

The OF1 board and OFOF1 case work with any MX-style mechanical switch.  The OFOF1 uses the screw-together button housings shown below.
![image](https://user-images.githubusercontent.com/95242582/177423209-cf4472c3-63f1-41cc-b781-756241bba0d2.png)
![image](https://user-images.githubusercontent.com/95242582/177423346-5b6b06be-8222-4141-91e2-8698a198bcd1.png)

To assemble, the switch is placed into the bottom half of the housing, and the top half is screwed into the bottom half through the hole in the top panel.  The keycap is then pressed onto the switch stem.  As with the standoffs, these can be printed at home or ordered from JLC.  Please note that you will need an o-ring around the top housing, under the panel (see Hardware section).

A panelized file is available that includes parts for 3 complete buttons (top half, bottom half, and keycap).  The LEDO6060 resin from JLC is the recommended material for these parts. For a full set, 7 copies of the file need to be ordered.  The files of the individual parts are also available
![image](https://user-images.githubusercontent.com/95242582/177424960-2e8d3128-e9a8-44c8-9dac-727e9f6e1b16.png)

Note: these housings are compatible with official Frame1 keycaps or any circular keycap that is 20.64mm or less in diameter.

For more information on 3D printing keycaps, check out: https://github.com/rana-sylvatica/circle-keycaps

The OFOF1_alt does not use these button housings, so any keycaps will work for that. Circular, square, etc are all fine.

## Hardware

Here's what is needed to assemble a full controller:

### OFOF1

x9 16mm Flanged Button Head Screw
https://www.mcmaster.com/90909A724/

x9 Narrow Base Weld Nut
https://www.mcmaster.com/90594A320/

x20 O-ring
https://www.mcmaster.com/9452K75/

### OFOF1-alt

x9 10mm Flanged Button Head Screw
https://www.mcmaster.com/90909A722/

x9 Narrow Base Weld Nut
https://www.mcmaster.com/90594A320/

## Additional info

If you wan to know more or discuss these designs, DM on discord at bjartskular1#6913 or join my server at https://discord.gg/9wBaMWgJkv
