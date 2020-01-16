# Automated Grains of Infinity production

Grains of Infinity is tedious to craft. Here is how I keep 5,000 of them in my ME system at all times.

![alt text][screenshot]

## Mods Used

* Applied Energistics 2
* Extra Utilities 2
  * Or any mod with a repeating redstone clock that can be disabled with a redstone signal
* EnderIO 
  * Or any mod with a vacuum chest, such as Thaumcraft's hungry chest, OpenBlocks vacuum hopper

## Materials pictured
* 1 Extra Utilities 2 Redstone Clock
* 1 Dispenser (vanilla)
  * Pointed down
* 1 EnderIO Vacuum Chest
* At least 1 Bedrock block
* 1 Applied Energistics Level Emitter, set to emit when levels are above or equal to limit (of however many Grains of Infinity items you wish to keep in stock)
* 1 Applied Energistics Export Bus, exporting Flint and Steel items from existing ME system into dispensor.
* 1 Applied Energistics Import Bus, to import contents of the vacuum chest into the existing ME system
* Lots of Flint and Steels, or the ability to auto-craft them

## Explanation
* Grains of Infinity are created by lighting fire on a bedrock block and letting the fire burn out naturally. When this happens, there is a chance to create a Grains of Infinity item.
* The redstone clock triggers the dispenser, which uses a Flint and Steel in the empty space below it, which should be Bedrock.
* The dispensor _won't_ actually trigger a flint and steel charge if there is already a fire underneath it, so it does not waste your flint and steel durability.
* The AE Export Bus keeps the dispenser stocked with Flint and Steel items. These last multiple uses, but they do wear out, and the item is not a guaranteed drop.
* The Grains of Infinity item will be on fire when it spawns, and _can_ burn up, so you need something to pull it out of the fire to collect it. Any Vacuum chest works best for this (does not have to be an EnderIO one)
* The level emitter emits a redstone signal into the Redstone Clock when the ME system has the desired amount of items in stock.
* This makes noise, so either assemble it away from your base, or use Sound Mufflers (Extra Utilities 2) to dampen the sound.

[screenshot]: ../Images/GrainsOfInfinity.png "Screenshot"