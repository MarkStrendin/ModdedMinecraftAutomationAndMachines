# Automated Sunflower production

I needed a large amount of sunflowers to create EnderIO's Liquid Sunshine. Here's how I made a system to keep 5000 in my ME system at all times.

![alt text][screenshot]

## Mods Used

* Applied Energistics 2
* Extra Utilities 2
  * Or any mod with a repeating redstone clock that can be disabled with a redstone signal
* EnderIO 
  * Or any mod with a vacuum chest, such as Thaumcraft's hungry chest, OpenBlocks vacuum hopper, or even just vanilla hoppers.

## Materials pictured
* 1 Extra Utilities 2 Redstone Clock
* 1 Dispenser (vanilla)
* 1 EnderIO Vacuum Chest
* 1 Dirt
* 1 Sunflower (planted on dirt block)
* 1 Applied Energistics Level Emitter, set to emit when levels are above or equal to limit (of however many sunflower items you wish to keep in stock)
  * Oriented to emit a signal into the Redstone Clock block, to stop it when the system has enough.
* 1 Applied Energistics Export Bus, exporting Bone Meal from existing ME system into dispensor.
  * My ME system knows how to craft bone meal from bones, and so this export bus has a Crafting Card, to make sure it stays topped up when supplies run out
* 1 Applied Energistics Import Bus (below the Vacuum Chest), to import contents of the vacuum chest into the existing ME system
* A light source (Extra Utilities Glowing Glass) to keep the flower from "popping off" because of light levels. 
  * I am not sure if this can actually happen, but I figured better safe than sorry. If it does, your vacuum chest will pick it up at least.
* Lots of Bone Meal - one bone meal per sunflower that you need, or ideally.
  * Creating any kind of mob farm that collects skeleton parts is a great way to have more bones than you know what to do with.

## Explanation
* Sunflowers will simply drop another sunflower item when you right click them with bone meal
* You can use a dispensor filled with bone meal to do this automatically
* You will need something to "catch" the additional sunflower items, as they will be dropped on the ground like an item.
* You can use an Applied Energistics Level Emitter to make sure that you always have a certain number of sunflower items "in stock". When the emitter emits a redstone signal, the clock stops, stopping the dispensor.
* Applied Energistics can keep the dispensor full of bone meal, especially if your system knows how to craft it
* The sunflower is not used up, and does not need to be replanted.


[screenshot]: ../Images/sunflower.png "Automated Sunflower screenshot"