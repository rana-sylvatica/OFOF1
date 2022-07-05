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

The files for the bottom panel, top panel, and alternate top panel are provided in DXF format (2D CAD), STEP format (3D CAD), and as Gerber PCB fabrication files.  

Outer dimensions of the panels are 14"x7".


## Standoffs

The standoffs that hold the layers at the proper spacing are designed to be 3D printed.  They can be printed at home or ordered using an online 3D printing service such as the one offered by JLCPCB.  If ordering from JLC, it is fine to use the cheapest option for resin (9000R), and make sure to use the versions of the files with x8 or x10 in the filename. 

![image](https://user-images.githubusercontent.com/95242582/177422742-10cc2180-853b-4335-b5df-835c6af1c75a.png)


A complete build requires 4 corner standoffs, 5 bottom standoffs, and 5 top standoffs.  Note that there are different versions of the corner and top standoffs for the OFOF1_alt build configuration.

Files for these are provided in STEP and STL format, both as individual parts for at-home printing and panelized parts for ordering.  

## Buttons

## Hardware
