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

>[!TIP]
>Trip world cart made in collab with RainDX

<img width="500" height="333" alt="mbc1tripworld" src="https://github.com/user-attachments/assets/12ede6a1-414d-42ca-ab6f-a48405845a33" />
<img width="500" height="333" alt="mbc1moneyidolexchanger" src="https://github.com/user-attachments/assets/9eeb5b57-3bd2-43ed-8fa3-9b42e366b043" />
<img width="500" height="508" alt="mbc1kicadrender" src="https://github.com/user-attachments/assets/7e633a03-44c4-4887-8f54-46d6b89ee1d1" />

Final Version. One for tinkering and one finished Trip World cart!
 
## Parts List

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
>Make sure your solder joints are of high quality to avoid problems.
 
I haven't put any local filtering for the logic as mostly there isn't room and I've seen no need for it. There is no save function so a game crash will ruin your progress but not ruin a save. Maybe it's needed, I don't know, so there is a single bypass capacitor up by the EPROM. I personally haven't populated it.
 
## Copies
 
Someone copied my design on TaoBao. They are likely based on my previous design which did include some mistakes!

>[!NOTE]
>I'm quite sure that these are no longer being sold, this was some years ago.
 
The boards look the same but they have some custom engraved EEPROMs to go with it. Those EPROMs should work just fine with this design if you wanted to have an extra cool touch.
 
<img width="412" height="676" alt="mbc1taobaocopy1" src="https://github.com/user-attachments/assets/5561ce09-a2b7-4a77-9e0d-1a002c50874c" />
<img width="500" height="328" alt="mbc1taobaocopy2" src="https://github.com/user-attachments/assets/9d778c42-94c4-43c1-b50d-f52b8bcbf7dd" />

## Links

🛍️ Inside Gadgets Shop: https://shop.insidegadgets.com <br>
📎 Inside Gadgets GitHub: https://github.com/insidegadgets <br>
📷 Inside Gadgets Insta: https://www.instagram.com/inside.gadgets <br>
🎥 RainDX Insta: https://www.instagram.com/rain__dx <br>
🖇️ Bytendo Mods GitHub: https://github.com/bytendomods <br>
🐭 Bucket Mouse: https://github.com/Bucket-Mouse <br>
🛒 Natalie Shop: https://nataliethenerd.com/ <br>
🤓 Natalie GitHub: https://github.com/natalie-lang/natalie <br>
☕ Jamo KoFi: https://ko-fi.com/jamo_mods <br>
📱 Natalie Discord: https://discord.gg/moddedgameboyclub <br>
🍵 My KoFi: https://ko-fi.com/sillyhatday <br>
😼 Lesser Kuma: https://github.com/lesserkuma <br>
