# How to assemble an OFOF1 (regular version)

## Step 1: Tools

Here is the bare minimum of what you will need:
 - Soldering iron
 - Solder
 - Flush cutters
 - Hobby knife
 - 3mm hex key

A multimeter is not technically required but will make your life easier

![IMG_20220919_144336040](https://user-images.githubusercontent.com/95242582/191127035-48e306d2-e20d-4eaf-afd6-1137bbc93b87.jpg)

---

## Step 2: Parts

Here are all the parts that you will need (the packing list shows what I pack in the DIY kits I sell and includes a few spares of button parts, hotswap sockets, hardware, etc.)

![IMG_20220919_144244734](https://user-images.githubusercontent.com/95242582/191128271-d5f80a61-0803-4af6-a925-84c978364552.jpg)

![packing list](https://user-images.githubusercontent.com/95242582/191128425-a0cd3940-fbf6-44fb-b83a-7e83cca368fc.png)

---

## Step 3: Buttons

### 3.1:

Break the button panels apart and sort the top housings, bottom housings, and keycaps
![IMG_20220919_144750126](https://user-images.githubusercontent.com/95242582/191128751-521e034b-088a-4000-8f39-13a1194efe8b.jpg)

### 3.2:

Use the flush cutters and/or the hobby knife to clip/cut the remaining connecting bits from the button parts

### 3.3: 

Insert a top housing through the hole in the top panel
![IMG_20220919_145837458](https://user-images.githubusercontent.com/95242582/191129148-25e63269-ccbd-4868-be7e-d092e77c5441.jpg)

### 3.4: 

Put an o-ring over the protruding portion of the top housing
![IMG_20220919_145906189](https://user-images.githubusercontent.com/95242582/191129198-b8f2a213-183d-402b-a017-f397ea0b268a.jpg)

### 3.5:

Screw the bottom housing onto the threads of the top housing until it is snug (not overly tight) and the square hole is parallel with the top panel

![IMG_20220919_145949179](https://user-images.githubusercontent.com/95242582/191129300-33e5d11c-032e-41f0-9175-985e353b180a.jpg)

### 3.6:

Repeat for the remaining 19 buttons.  When finished it should look like this:
![IMG_20220919_151228537](https://user-images.githubusercontent.com/95242582/191129349-7c30c110-f85f-4aa0-bfa9-663068c01844.jpg)
![IMG_20220919_151237929](https://user-images.githubusercontent.com/95242582/191129355-e179f4ee-e064-448a-a2d8-47c09d09b8e2.jpg)

### 3.7

Insert switches into all the housings as shown - make sure the pins are aligned towards the bottom of the panel to fit with the hotswap sockets on the OF1 PCB

Do not put keycaps on yet

![IMG_20220919_151611608](https://user-images.githubusercontent.com/95242582/191129630-3dda2c8e-2469-4810-ad21-0845d0d12a63.jpg)

---

## Step 4: Soldering

There are two methods of soldering the pico onto the OF1 PCB.  **The first method is for experienced solderers only.** If you do not feel very comfortable soldering or do not have a mulitmeter, I recommend the second method.

### Method 1:

Put a small amount of solder onto the USB data pads under the pico

![IMG_20220919_151950707](https://user-images.githubusercontent.com/95242582/191130050-61fb0a19-652f-43e5-9457-bedb01164d3e.jpg)

Attach the pico to the OF1 board with tape or by soldering one of the debug pins to tack it in place. Turn the board over and solder the data pads through the plated holes as shown, while pressing down on the board.  The solder on the pads on the pico should flow into the plated holes but you may need to add a little bit of additional solder to get enough heat flow.
![IMG_20220919_152302809](https://user-images.githubusercontent.com/95242582/191130241-c4407b70-9edd-4c05-bb77-6034531d879f.jpg)

After doing this and before soldering the rest of the pins, check continuity with a multimeter between the pins on the pico USB (circled on the left) and the d+ and d- pins on the OF1 board (circled on the right).  Also make sure the data pins do not have continuity to each other. 

![IMG_20220919_152700049](https://user-images.githubusercontent.com/95242582/191130593-b8af78ab-6443-401b-ae3f-c6a53b6df5a8.jpg)

Use this image as reference for finding d+ and d- on the pico USB

![image](https://user-images.githubusercontent.com/95242582/191130763-cfaa3987-221b-4743-9a97-65a2be92b336.png)

Finally, solder the rest of the pins.  Finished result should look something like this:

![IMG_20220919_153250754](https://user-images.githubusercontent.com/95242582/191130803-f84a74b4-809f-4a58-959a-4d99301975f7.jpg)

### Method 2:

Instead of surface mounting the pico to the OF1 board, you can buy a Micro USB to USB C cable and pin headers, which greatly reduces the chances for soldering issues that are difficult to fix.  Below are links to examples that will work well for this (not provided in the DIY kit but recommended to purchase if you are a novice solderer)

https://www.amazon.com/dp/B0744BKDRD

https://www.amazon.com/MCIGICM-Header-2-45mm-Arduino-Connector/dp/B07PKKY8BX

Doing it this way will look like this. Just solder the pin headers into the OF1 PCB and then solder the pico onto the headers, and plug the cable into the pico and the secondary USB C port on the OF1 PCB. 

![IMG_20220919_152121047](https://user-images.githubusercontent.com/95242582/191131095-aa297981-7de1-4273-92d8-630a4ac40673.jpg)

