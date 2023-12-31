# GAMEBOY-FLASHCART-MBC1-DISCRETE
A Gameboy flashcart using discrete logic as a MBC1 replacement

Using footprints from https://github.com/HDR Be sure to check out their designs as well.

This a tested working flashcart design that was created from a schematic found on the internet. This schematic has been floating around the web since the 90's but I've 
only seen one person try to make a cartridge using that design. This is done with surface mount 74XX series logic that is new and current. I made this to suit want I wanted
as I came across a pile of 64KB EPROMs for free and made a cartridge to use them. Well this is basically an evolution of that using 512KB EPROMs. The EPROMs are no longer made 
as far as I can see, but they are available across eBay and Aliexpress.

The downside of this design is that EPROMs are erased in a UV eraser and programmed in a dedicated programmer. This is a lot less convienient for most people versus something like the GBxCart RW.
The EPROM also does not fit into the cartridge shell, sticking out from the top of the cartridge. I quite like the way the EPROM sticks out from the top of the cartridge, it has a cyberpunk or prototype look to it.

Due to Chinese copies, I added "original" to the back of my cart, just so you can feel smug about having the original design.

![Gameboy 512KB Cart Discrete Logic Front](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/546adfbd-cc16-4f19-87f0-4a89dede614f)

![Gameboy 512KB Cart Discrete Logic Back](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/b29cd008-b40e-429b-b887-79f1b87ca9d7)

![IMG_5681](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/fdd5c244-bbce-4291-b9f8-f7a260b6721f)
![IMG_5637](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/de99a0bb-a1df-40f3-9fa1-70af790dc962)

Final Version. One for tinkering and one finished Trip World cart!

**EPROM**

The EPROM I use is the nice ceramic package 27C040. Very old school look and feel. It is certainly in like with the look and technology of the Gameboy. They are not cheap but also not expensive,
 so you can get a bunch of them in a storage container and switch the EPROM out from the cartridge as you wish. For this reason I reccomend putting the EPROM in a socket.
 Make sure to use a quality chip socket as I've found the connections to be very sensitive to the Gameboy. A quality socket will remove all worry about that. Also remember when soldering the socket to trim the pins short before soldering. You will need to do this to keep the back of the PCB flat against the back of the cartridge. It's not ideal but thats the nature of using through hole components where you should be using surface mount.
 
 **Discrete Logic**
 
 You'll need 5 seperate 74XX logic chips to replicate the bank switching of an MBC1.
 | Part No | Description | Amount |
 | --- | --- | --- |
 | 74HC32 | Quad 2 input OR Gate | 1 |
 | 74HC27 | 3 Input NOR Gate | 1 |
 | 74HC174 | Hex D Type Flip Flop | 1 |
 | 74HC08 | Quad 2 Input AND Gate | 1 |
 | 74HC00 | Quad 2 Input NAND Gate| 1 |
 | 32 DIP SKT | EPROM Socket | 1 |
 | 100nf Cap | 0603 | 1 |
 
 Make sure to get really nice solder joints when putting these on. I've seen perfect looking joints that do no make connection. Any problems when first trying out the cartridge, reflow all the 74XX chip legs.
 
 I haven't put any local filtering for the logic as mostly there isn't room and I've seen no need for it. There is no save function so a game crash will ruin your progress but not ruin a save. Maybe it's needed, I don't know, so there is a single bypass capacitor up by the EPROM. I personally haven't populated it.
 
 **Compatability**
 
 Every single MBC1 based game under 512KB that doesn't require saving works perfectly. Well that is the theory, but I've tried a bunch of games and they all work great. This is great for early games from the Gameboys life. Mostly they didn't have a save function back then, so you just remembered your high scores. Look in the COMPAT file for games I have tested myself.
 
 **Copies**
 
 I've seen that China has copied this design. They seem to be for sale on TaoBao. Look out for these. They are likely based on my previous design which did include some mistakes!
 
 The boards look the same but they have some custom engraved EEPROMs to go with it. Those EPROMs should work just fine with this design if you wanted to have an extra cool touch.
 
 ![MBC1 Copy](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/e559b3f1-7cf5-447c-8597-5a02b1b501f9)
![MBC1 Copy Chips](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/38d28594-3082-4a77-adda-fae669a4a791)

**Also**

Check out these links:

https://ko-fi.com/jamo_mods

https://discord.gg/moddedgameboyclub

https://ko-fi.com/sillyhatday

https://github.com/lesserkuma

https://github.com/HDR
