# How to assemble an OFOF1 (regular version)

These are the instructions for building your very own OFOF1 controller.  If you can assemble a LEGO set and can do a bit of basic soldering, this will be very doable.  It should take about 2 hours for a first time builder to go from kit to finished controller.


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



Break the button panels apart and sort the top housings, bottom housings, and keycaps
![IMG_20220919_144750126](https://user-images.githubusercontent.com/95242582/191128751-521e034b-088a-4000-8f39-13a1194efe8b.jpg)



Use the flush cutters and/or the hobby knife to clip/cut the remaining connecting bits from the button parts



Insert a top housing through the hole in the top panel
![IMG_20220919_145837458](https://user-images.githubusercontent.com/95242582/191129148-25e63269-ccbd-4868-be7e-d092e77c5441.jpg)



Put an o-ring over the protruding portion of the top housing
![IMG_20220919_145906189](https://user-images.githubusercontent.com/95242582/191129198-b8f2a213-183d-402b-a017-f397ea0b268a.jpg)



Screw the bottom housing onto the threads of the top housing until it is snug (not overly tight) and the square hole is parallel with the top panel

![IMG_20220919_145949179](https://user-images.githubusercontent.com/95242582/191129300-33e5d11c-032e-41f0-9175-985e353b180a.jpg)



Repeat for the remaining 19 buttons.  When finished it should look like this:
![IMG_20220919_151228537](https://user-images.githubusercontent.com/95242582/191129349-7c30c110-f85f-4aa0-bfa9-663068c01844.jpg)
![IMG_20220919_151237929](https://user-images.githubusercontent.com/95242582/191129355-e179f4ee-e064-448a-a2d8-47c09d09b8e2.jpg)



Insert switches into all the housings as shown - make sure the pins are aligned towards the bottom of the panel to fit with the hotswap sockets on the OF1 PCB

Do not put keycaps on yet

![IMG_20220919_151611608](https://user-images.githubusercontent.com/95242582/191129630-3dda2c8e-2469-4810-ad21-0845d0d12a63.jpg)

---

## Step 4: Soldering the pico

There are two methods of soldering the pico onto the OF1 PCB.  **The first method is for experienced solderers only.** If you do not feel very comfortable soldering or do not have a mulitmeter, I recommend the second method.

Before starting either method, it is a good idea to program the pico and make sure it works.  Plug it in to your computer with a micro USB cable and follow the instructions at https://github.com/JulienBernard3383279/pico-rectangle/ or https://github.com/JonnyHaystack/HayBox.  If the pico does not show up on the computer when initially plugged in, it is defective and you should get a new pico.

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
 
---
 
## Step 5: Soldering the hotswaps and assembling the case

After soldering the pico, return to the top panel with button housings and switches.  Placing it face-up, insert the 16mm M5 screws into the 5 inner holes in the panel, ignoring the corners for now.  Place small bits of painter's tape over the switches to keep them in place.

![IMG_20220919_153411943](https://user-images.githubusercontent.com/95242582/191131494-0fc44862-5984-4db5-99b7-e7594e58585d.jpg)

Take the top standoffs and break them apart and clean off the connecting bits

![IMG_20220919_153428931](https://user-images.githubusercontent.com/95242582/191131567-c216941a-c198-42d5-a890-aad75045c523.jpg)

Turn the top panel over and place the standoffs as shown onto the 5 screws

![IMG_20220919_153527226](https://user-images.githubusercontent.com/95242582/191131611-678ae9cc-5777-470a-9598-b2ab8dcccf21.jpg)

Place the OF1 PCB onto the switches/standoffs as shown.  Ensure that the pins of the switches are not bent.

![IMG_20220919_153558694](https://user-images.githubusercontent.com/95242582/191131726-8c22ab5e-a4eb-494d-ba14-cfa65ae26174.jpg)

Place the hotswap sockets on the switch pins and push them into place.  You may need to lift up the top panel and squeeze between the switch and the hotswap socket to make sure they are both properly seated.  The socket should rest flush against the OF1 PCB.

![IMG_20220919_153927565](https://user-images.githubusercontent.com/95242582/191132080-8fd392a6-ff18-4145-badb-83a8efbb1b0e.jpg)

Solder the hotswap sockets to the board. Done properly the should look like this:
![IMG_20220919_154246548](https://user-images.githubusercontent.com/95242582/191132115-6bccd1a2-4281-45ce-9789-d41937fbbb42.jpg)

Take the bottom standoffs and break them apart and clean off the connecting bits, then place them on the OF1 PCB, over the 5 screws as shown.

![IMG_20220919_154308236](https://user-images.githubusercontent.com/95242582/191132499-ca487b2f-7ca8-488c-ac25-153f54bc099c.jpg)


![IMG_20220919_154352544](https://user-images.githubusercontent.com/95242582/191132272-d7ee5d3b-b295-4908-8d49-0b71703f5ee1.jpg)

Place the bottom panel on top of the bottom standoffs and gently screw on M5 weld nuts onto the screws in the 5 inner holes as shown.  They do not need to be tight, just enough to hold the whole thing together.

![IMG_20220919_154446332](https://user-images.githubusercontent.com/95242582/191132411-51814e7c-50a3-4155-8382-5f69b912d776.jpg)

Break apart and clean the corner standoffs, and then place them in each corner.  Place a weld nut through each corner hole and cover with a bit of painter's tape to hold in place.

![IMG_20220919_154454883](https://user-images.githubusercontent.com/95242582/191132511-27f5aa9e-71bc-40d0-9ab9-6025bc474d3f.jpg)
![IMG_20220919_154615678](https://user-images.githubusercontent.com/95242582/191132565-432adbe4-5dca-4bfd-8f61-1d78cb8d1dfa.jpg)

Turn the controller over, remove the painter's tape from the screws on the top panel, place screws in the four corners, and tighen all screws with the 3mm hex key.

Ensure everything is lined up correctly before tightening.

![IMG_20220919_154811438](https://user-images.githubusercontent.com/95242582/191132640-0effee1f-838f-4110-bda0-2d7c2b05e935.jpg)

Turn the controller over and remove the painter's tape from the corner weld nuts.  Take the anti-slip foam pad and peel it off the paper backing.


![IMG_20220919_154901421](https://user-images.githubusercontent.com/95242582/191132784-2f932007-1425-4906-9c58-cb70693e8300.jpg)

Stick on the bottom panel as shown.  The adhesive is fairly strong so be careful to line it up correctly.
![IMG_20220919_155029987](https://user-images.githubusercontent.com/95242582/191132816-32ab5bd9-b9ad-4a5d-81f7-03d353e8d25e.jpg)

Turn the controller back over, and place the keycaps on the switches.

![IMG_20220919_155301853](https://user-images.githubusercontent.com/95242582/191132859-b5218d5c-82b5-4c07-ae2d-b8f615e66ddd.jpg)

Congratulations! You finished your OFOF1!

