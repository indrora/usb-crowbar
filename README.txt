 ...    ::: .::::::. :::::::.          .,-::::: :::::::..       ...    .::    .   .::::::::::.    :::.    :::::::..   
 ;;     ;;;;;;`    `  ;;;'';;'       ,;;;'````' ;;;;``;;;;   .;;;;;;;. ';;,  ;;  ;;;'  ;;;'';;'   ;;`;;   ;;;;``;;;;  
[['     [[['[==/[[[[, [[[__[[\.      [[[         [[[,/[[['  ,[[     \[[,'[[, [[, [['   [[[__[[\. ,[[ '[[,  [[[,/[[['  
$$      $$$  '''    $ $$""""Y$$ cccc $$$         $$$$$$c    $$$,     $$$  Y$c$$$c$P    $$""""Y$$c$$$cc$$$c $$$$$$c    
88    .d888 88b    dP_88o,,od8P      `88bo,__,o, 888b "88bo,"888,_ _,88P   "88"888    _88o,,od8P 888   888,888b "88bo,
 "YmmMMMM""  "YMmMY" ""YUMMMP"         "YUMMMMMP"MMMM   "W"   "YMMMMMP"     "M "M"    ""YUMMMP"  YMM   ""` MMMM   "W" 


The USB Crowbar is a footprint replacement for the venerable USB-B full size connector. 

The vast majority of right-angle board-mount USB Type B connectors have the same footprint, down to the shape
and size of the pads, body, etc. 

A friend of mine was tired of the USB connectors failing on her DJ equipment after just a few years. Sometimes,
that was juast a few shows over a few months. 

Skill issue on my part, I said the words "This should be easy".

Reader: it was not easy.

You can buy these in sticks of five from my Tindie store: https://www.tindie.com/products/indrora/usb-crowbar/


--- DETAILED INSTALLATION INSTRUCTIONS ---

1. Verify that the USB B connector on your device is compatible: It must be right angle (that is, it plugs in
   parallel to the board surface, rather than jamming into it), and must have the angled side of the plug at
   the top ("away" from the board). Generally, it should look like what's on the Arduino Uno. Wikimedia
   has a pretty good picture of what you're looking for: https://commons.wikimedia.org/wiki/File:Arduino_Uno_005.jpg
   This is *not* compatible with vertical USB connectors like the one in this photo of a Rigol oscilloscope:
   https://commons.wikimedia.org/wiki/File:Rigol_DS1054Z_Oscilloscope_Teardown_PCB_(15354017188).jpg
   https://commons.wikimedia.org/wiki/File:Rigol_DS1054Z_Oscilloscope_Teardown_PCB_(15537475561).jpg (on the right hand side)

2. Desolder your connector. Hints:
   - Add a touch of fresh solder.
   - Remove as much solder from the shield strain relief pins as you can, then trim them flat. Heat the board
     gently with a hair dryer or hot air to help reduce heat loss.
   - In my experience, once you have the four signal pins handled, you're golden. Use whatever means you need to remove the
     connector. Sometimes, this has meant being Destructive. 

3. Using 22ga wire, solder two U-shaped loops through the top of the crowbar.
4. Line up the crowbar with the footprint of the original USB connector. Tack in place one of the structural joints on the sides.
5. Solder the thru-wires on the backside of the board
6. Trim the bottom and top sides, removing excess wire. Trim the wires on the top of the crowbar as flush as you can.

/!\ At this point, you can safely test the connection.

7. Flood the structural joints on the sides with solder. It shouldn't want to lift. 
8. Clean with alcohol and allow to dry. 

-- FREQUENTLY QUESTIONED ANSWERS --

Q: MiniB? MicroB?

I've had a *ton* of requests for this. Unfortunately, it's not in the cards. 

* The physical dimensions of a USB Type C connector are against us: It's huge!
* There's maybe 3 total layouts for USB2 Type B (two thru-hole and one surface mount) that I've found. Most others are within 0.5mm of that in some dimension, with the pinout being the exact same for thru-hole versions. 
* The USB C connector housing *happens* to be exactly the width of the USB Type B connector.

Both Mini and Micro-B have a lot of different layouts (4/5 pin variants, thru-hole and SMT, different landing pads for the shell vs. sunk holes for the shell, etc.). This hasn't stopped one intrepid friend of mine who replaced the Micro-B connector on something by using 24ga stranded core wire and very carefully bodging the required lines. If you can make the space for the connector to cram it down, Do It! 

In some cases, since the connector is on a separate board, it may well be reasonable to design a replacement board for the USB connector, as was done in the case for the PS4 Controllers. Marcus Heier has a fantastic drop-in modification for several generations of PS4 controllers that you can buy from him on Tindie: https://www.tindie.com/products/mariusheier/ps4-controller-usb-c/ -- you can see the process of installing it here: https://youtu.be/o9IACHF22yc

Q: USB Type A????

One of the inspirations for this project was Palconn's USB A compatible ports: http://palconn.net/products/?id=100

Finding them is a bit tricky...

-- LICENSE --

This work is licensed under CC-BY.

I have a dream that some day, I will be able to buy these from vendors such as Palconn and Samtec as retrofits for old designs.
If you're in that scene, hmu ;) 
