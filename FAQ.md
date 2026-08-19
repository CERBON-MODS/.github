## General

**Q: Can I use the mod in my mod pack?**

A: Yes, you can.

**Q: Are you going to backport the mod to older versions?**

A: All my mods that are currently using the multiloader template won't be backported to versions below 1.20.1. New mods released after 1.20.1 may or may not be backported.

## Bosses of Mass Destruction

**Q: Can you add X or change Y?**

A: I prefer keeping the mod as similar as possible to the original. So, I advise you to ask the original mod author, [here](https://github.com/miyo6032/bosses-of-mass-destruction). If they decide to implement the feature, I will add it.

**Q: Is there a Fabric version?**

A: Yes, you can get it [here](https://www.curseforge.com/minecraft/mc-mods/bosses-of-mass-destruction). The Fabric version is the original, my mod is only a port.

## Better Totem of Undying

**Q: I have blacklisted a dimension/structure and it's not working. Why?**

A: Probably you have written the dimension/structure ID incorrectly. Please double-check if you have entered the correct mod ID and dimension/structure ID. Another possibility is that you haven't saved the file.

**Q: Is it possible to blacklist damage types?**

A: Yes, it is. You can do it by adding the damage types you want to the `bypasses_invulnerability` tag using a [datapack](https://minecraft.fandom.com/wiki/Tutorials/Creating_a_data_pack). It's located at `minecraft\tags\damage_type\bypasses_invulnerability.json`.

**Q: How do I add blocks to the "totem_cant_break" tag?**

A: You need to [create a datapack](https://minecraft.fandom.com/wiki/Tutorials/Creating_a_data_pack) and use the following path: `data/better_totem_of_undying/tags/blocks` and create at this location the file `totem_cant_break.json`. Then add to the json file the blocks you want.

**Q: How do I add custom effects?**

A: Custom effects cannot be configured through the GUI. Instead, you will need to open the config file directly. In this file, you will find a configuration called `custom_effects`. Use this list to add custom effects and specify their triggers. Within this list, provide another list enclosed in curly braces. The first parameter should be the damage type, the second parameter the effect to be granted, the third parameter the duration of the effect in ticks, and the fourth parameter the effect amplifier. If you want the effect to be granted regardless of the damage type, use `any`. For example: `[["minecraft:out_of_world", "minecraft:blindness", "800", "0"]]`. In this example, if the player dies in the void, the totem will grant a level 1 blindness effect with a duration of 40 seconds.

## Better Beacons

**Q: I have a problem adding blocks/items to a tag or to the newest datapack folders. What should I do?**

A: Please read the [wiki](https://github.com/CERBON-MODS/CERBONs-Better-Beacons-FORGE/wiki) and if you cant solve your problem, you can contact me directly on my [discord server](https://discord.gg/2PvYZfjWDf).

