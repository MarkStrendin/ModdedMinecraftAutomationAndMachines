# Automated Applied Energistics Pure / Fluix Crystals

![alt text][screenshot1]
![alt text][screenshot2]

## Mods Used

* Applied Energistics 2


## Materials pictured
* 4 Crystal Growth Accellerators
* 1 Water source block
* 1 ME Formation Plane (On top of water source block)
* 1 ME Annihilation Plane (On bottom of water source block)
* 2 Quartz Fiber (to separate this structure into 3 seperate ME networks)
* 3 ME Interfaces
* 1 ME Import Bus
* 1 ME Chest
* 1 1K Storage Cell (in ME Chest)
* 10-20 ME Cable

## Explanation
* You want to create **2** completely seperate ME networks, seperate from your main ME network.
  * One network that handles inputting crystal seeds into the water
    * Pictured with *Orange* cable
    * Contains only an ME Interface, an ME Formation Plane, and the orange cables between those two
    * Separated from the other networks using a Quartz Fiber, so that it can still draw power from them
  * One network that collects the completed crystals, storing them, and providing them to your main network
    * Pictured in *Light Blue* cables
    * Contains an ME chest with a 1K storage cell. The storage cell should be partitioned using a Cell Workbench to only accept completed pure crystals and fluix crystals.
    * Contains an ME Interface to provide contents to main network
    * Separated from the other networks using a Quartz Fiber, so that it can still draw power from them
    * If the storage cell is partitioned properly, the annihilation plane will leave unfinished crystal seeds in the water, but will accept the completed crystals
    * The ME Interface should be configured to provide the completed crystals (using the top slots of the interface)
* The ME Import bus and *green* cabling represents the main ME network
* The Green ME Interface holds crafting patterns to convert 1 seed of a given crystal type into 1 pure crystal. The interface accepts the seeds, which get dropped into the water from the formation plane. When the seeds completely grow into crystals, the annihilation plane accepts them into the storage chest, and the light blue interface offers them to the green import bus, which then imports them into your main ME network

[screenshot1]: ../Images/ae_pure_crystals_1.png "Screenshot 1"
[screenshot2]: ../Images/ae_pure_crystals_2.png "Screenshot 2"