# Introduction

A Gameboy flashcart using discrete logic as a MBC1 replacement.

>[!NOTE]
>No game save support.

This is my first dive into how old cartridges work. I came accross a pile of ceramic 64KB EPROMs. Looked them up and thought, I wonder if I connect them to the gameboy cartridge bus it will work...

This a tested working flashcart design that was created from a schematic found on the internet. This schematic has been floating around the web since the 90's but I've 
only seen one person try to make a cartridge using that design.

Using some logic gates, the MBC1 mapper is partially implemented. This circuit implements the ROM banking for up to 512KB of ROM space. This is the normal mode for MBC1 games, there are very few that use the 2MB mode. There is no circuitry to enable game saving. For that you will need to use a different cartridge, such as my [MBC1 flashcart](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-512KB) (Currently in dire need of an update).

>[!NOTE]
>This is not compatible with GBxCart & FlashGBX. It requires a programmer such as the TL866ii and a UV EPROM eraser.

This is not the most practicle cart due to the giant EPROM and equipment needed to program/erase it. It's just for the unique look.

Due to Chinese copies, I added "original" to the back of my cart, just so you can feel smug about having the original design.

## Game compatibility:

This will run any MBC1 game that doesn't require saving. It will run a lot of those games too but obviously you can't save your progress.

Some favourites of mine to run on here are, the Kirby games, Trip world & Money Idol Exchanger. There are some real good games out there from this early stage in the Gameboy life.

## Photos:

![Gameboy 512KB Cart Discrete Logic Front](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/546adfbd-cc16-4f19-87f0-4a89dede614f)

![Gameboy 512KB Cart Discrete Logic Back](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/b29cd008-b40e-429b-b887-79f1b87ca9d7)

![IMG_5681](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/fdd5c244-bbce-4291-b9f8-f7a260b6721f)
![IMG_5637](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/de99a0bb-a1df-40f3-9fa1-70af790dc962)

Final Version. One for tinkering and one finished Trip World cart!
 
 **Discrete Logic**

 >[!NOTE]
> You'll need 5 seperate 74XX logic chips to replicate the bank switching of an MBC1.
 
 | Part No | Description | Amount |
 | --- | --- | --- |
 | 74HC32 | Quad 2 input OR Gate | 1 |
 | 74HC27 | 3 Input NOR Gate | 1 |
 | 74HC174 | Hex D Type Flip Flop | 1 |
 | 74HC08 | Quad 2 Input AND Gate | 1 |
 | 74HC00 | Quad 2 Input NAND Gate| 1 |
 | 32 DIP SKT | EPROM Socket | 1 |
 | 100nf Cap | 0603 | 1 |

>[!TIP]
>Make sure your solder joints are of high quality. I've seen perfect looking joints that do no make connection.
 
I haven't put any local filtering for the logic as mostly there isn't room and I've seen no need for it. There is no save function so a game crash will ruin your progress but not ruin a save. Maybe it's needed, I don't know, so there is a single bypass capacitor up by the EPROM. I personally haven't populated it.
 
## Copies
 
Someone copied my design on TaoBao. They are likely based on my previous design which did include some mistakes!

>[!NOTE]
>I'm quite sure that these are no longer being sold, this was some years ago.
 
The boards look the same but they have some custom engraved EEPROMs to go with it. Those EPROMs should work just fine with this design if you wanted to have an extra cool touch.
 
![MBC1 Copy](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/e559b3f1-7cf5-447c-8597-5a02b1b501f9)
![MBC1 Copy Chips](https://github.com/sillyhatday/GAMEBOY-FLASHCART-MBC1-DISCRETE/assets/65309612/38d28594-3082-4a77-adda-fae669a4a791)

## Links

🛍️ Inside Gadgets Shop: https://shop.insidegadgets.com <br>
📎 Inside Gadgets GitHub: https://github.com/insidegadgets <br>
📷 Inside Gadgets Insta: https://www.instagram.com/inside.gadgets <br>
🖇️ Bytendo Mods GitHub: https://github.com/bytendomods <br>
🐭 Bucket Mouse: https://github.com/Bucket-Mouse <br>
🛒 Natalie Shop: https://nataliethenerd.com/ <br>
🤓 Natalie GitHub: https://github.com/natalie-lang/natalie <br>
☕Jamo KoFi: https://ko-fi.com/jamo_mods <br>
📱Natalie Discord: https://discord.gg/moddedgameboyclub <br>
🍵My KoFi: https://ko-fi.com/sillyhatday <br>
😼Lesser Kuma: https://github.com/lesserkuma <br>
