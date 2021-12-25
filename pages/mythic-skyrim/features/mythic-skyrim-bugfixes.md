---
title: Fixes
summary: Overview of some vanilla game bugfixes integrated with Mythic Skyrim.
permalink: mythic-skyrim-bugfixes.html
sidebar: mythic-skyrim-sidebar
toc: true
folder: mythic-skyrim
datatable: true
---


## USSEP

[Unofficial Skyrim Special Edition Patch] (USSEP) fixes hundreds of gameplay, quest, NPC, object, item, text and placement bugs with the goal to eventually fix every bug with Skyrim Special Edition not officially resolved by the developers to the limits of the Creation Kit and community-developed tools. Click this link to view the updated and complete [USSEP Changelog].

[Unofficial Skyrim Creation Club Content Patches] (USCCCP) is a bundle of patches to fix the bugs in the Skyrim Creation Club content as well as resolve conflicts between Creation Club mods and USSEP.

Mythic Skyrim integrates and supports all Creation Club content. Care was taken to ensure other mods integrated into the modlist remained USSEP compatible.

It is important to note that USSEP does not make any fixes that would require SKSE. For fixes that require SKSE, consult the table below.


## Mesh & Texture Fixes

<details>
  
<summary>Weapons Armor Clothing and Clutter Fixes</summary>
<br>
This is a test.
  
</details>

Weapons Armor Clothing and Clutter Fixes
- Corrects many of the bugs found in the vanilla weapon, armor, clothing, jewelry, and clutter records.
- Improves consistency and balance between different items (value, weight, damage, keywords, etc).
- Weapons and armor will scale in a predictable and consistent manner.
- The strength of an enchantment on a piece of enchanted jewelry is now properly reflected by the quality of the base jewelry.
- Perks that didn't apply consistently to all items in the game have been fixed.
- Female clothing variants will now use the correct texture in first-person.
- Changes the crafting categories to help organize and declutter the crafting menus.
- Increases the speed of arrows and bolts by 50% and makes them fly at a slightly flatter trajectory.
- Changes the stats and keywords for the dragon priest masks to better balance them with other gameplay options.
- Adjusts the stats of Dwarven, Elven, and Orcish weapons to make them consistent with the rank and quality of their respective armors and the progression of the Smithing perks.
- Switches the values and stats of Daedric and Dragonbone weapons, so that Daedric are the more powerful.
- Some previously unplayable or inaccessible items are now playable and/or accessible in game.
- Allows circlets to be worn with hoods.
- Almost all instances of hooded robes have been removed from the game and replaced with separate robe and hood combinations.
- Adjusts the loot found in certain furniture containers to be consistent with both the class and the type of furniture.
- Certain items have been renamed for easier sorting or to better fit the in-game appearance of that item.
- Necklaces and/or rings that were invisible when worn with certain clothing can now be seen.
- Potion bottles will now use the correct meshes, and Poison bottles will no longer appear flat and dull.

Armor Mesh Fixes SE
- Clipping, skinning, other bad deformations
- Bad normals and tangents
- Various mesh fixes, including missing partitions and incorrect meshes

Assorted Mesh Fixes
- Incorrectly flagged meshes not casting shadows, receiving shadows
- Incorrectly flagged meshes not contributing to depth buffer, and thus has incorrect depth of field
- Incorrectly flagged meshes not being reflected in water
- Missing/inaccurate collision
- Bad normals and tangents
- Strange lighting flags
- Bad geometry causing Z-fighting
- Broken UVs


## SKSE Fixes

There are many bugs in the vanilla game that require SKSE to resolve.

You can search to see if a particular bug from the vanilla game not handled by USSEP has been addressed by another mod in the search bar below.

The purpose of this table is to ensure there are no redundancies or conflicts in included vanilla bugfixes, without needing to cross-reference many mod page descriptions.


----
<div class="datatable-begin"></div>

Name    						                    | Mod                        | Description
--------------------------------------- | -------------------------- | -----------
Actor Value Percentage	                | Scrambled Bugs             | Fixes incorrect values being displayed in the HUD for player and NPC actor values (health, stamina, etc.) due to the target having any temporary buffs or debuffs to the relevant actor value.
Apply Spell Perk Entry Points: Arrows   | Scrambled Bugs             | Fixes the Bullseye perk from incorrectly applying at the start of killcams.
Harvested Flags                         | Scrambled Bugs             | Fixes flora and trees that have respawned in a loaded from being incorrectly harvested once again. This is an alternative to the Flora Respawn Fix.
Hit Effect Race Condition               | Scrambled Bugs             | Fixes race condition from preventing hit effects being applied to an actor if their mesh loads after a magic effect is first updated.
Magic Effect Conditions                 | Scrambled Bugs             | Fixes a floating-point error that will gradually prevent the conditions of magic effects from being updated. The longer a magic effect has been running for, the more frequently this will occur (article﻿). This is an alternative to the ability condition fix in Bug Fixes SSE.
Magic Effect Flags                      | Scrambled Bugs             | Fixes magic effects not respecting their flags when scaling their duration and magnitude.
Mod Armor Weight Perk Entry Point       | Scrambled Bugs             | Fixes the Mod Armor Weight perk entry point from not modifying the weight of just the armor you are wearing, but incorrectly modifying the weight of stacks of that armor.
Quick Shot                              | Scrambled Bugs             | Fixes the Quick Shot perk not being accounted for when calculating the power of an arrow fired by the player.
Terrain Decals                          | Scrambled Bugs             | Fixes decals not being applied to the terrain in cells that have been partially unloaded.
Training Menu Text                      | Scrambled Bugs             | Fixes the cost of a lesson displayed in the training menu not being affected by any buffs or debuffs to the relevant skill.
Weapon Charge                           | Scrambled Bugs             | Fixes the charge of equipped enchanted weapons only being restored to the charge they were when last equipped or recharged.
Enchantment Cost                        | Scrambled Eggchantments    | Fixes the value of player enchanted items and the amount of charge that player enchanted weapons is drained not being saved (article). This is an alternative to the Enchantment Reload Fix.
Multiple Enchantment Effects            | Scrambled Eggchantments    | Your skill in enchanting improves each of an enchantments effects, instead of only the costliest effect. This affects enchantments with multiple effects
ArcheryDownwardAiming                   | SSE Engine Fixes           | Fix a bug where projectiles sometimes don't fire properly if you're aiming downward. Ported from Cobb's LE fix. (see here)
AnimationLoadSignedCrash                | SSE Engine Fixes           | Fix an improper unsigned/signed conversion. Should allow loading more animations before a CTD 
BethesdaNetCrash                        | SSE Engine Fixes           | Fixes a crash on startup caused by improper handling of non-ASCII characters in Bethesda.net HTTP response headers. 
BSLightingAmbientSpecular               | SSE Engine Fixes           | Fixes a bug where lighting template Directional Ambient Specular & Fresnel Power are broken. 
BSLightingShaderForceAlphaTest          | SSE Engine Fixes           | Forces alpha testing in the lighting shader. Fixes object LOD reflections on water.
BSLightingShaderParallaxBug             | SSE Engine Fixes           | Fixes a bug with parallax lighting shaders
CalendarSkipping                        | SSE Engine Fixes           | Fixes the bug listed under Notes on this page
DoublePerkApply                         | SSE Engine Fixes           | Fixes a bug where NPCs in the player's cell will have their perk effects applied twice on game load
EquipShoutEventSpam                     | SSE Engine Fixes           | Fixes a bug where the 'Equip Shout' script would fire a shout equipped event even if the equip failed.
GHeapLeakDetectionCrash                 | SSE Engine Fixes           | Fixes a crash where scaleform attempts to report a memory leak but the code doesnt exist in Skyrim.
LipSync                                 | SSE Engine Fixes           | Fixes the lip sync bug, same as LE bug fixes.
MemoryAccessErrors                      | SSE Engine Fixes           | Fixes a handful of out-of-bounds or use-after-free bugs. Required for experimental memory patches.
MO5STypo                                | SSE Engine Fixes           | Fixes a typo in the ARMA (Armor Addon) form loader preventing 1st person female alternate texture sets from being loaded.
PerkFragmentIsRunning                   | SSE Engine Fixes           | See Misc Fixes SSE's readme﻿ for details.
RemovedSpellBook                        | SSE Engine Fixes           | See Misc Fixes SSE's readme﻿ for details
SaveScreenshots                         | SSE Engine Fixes           | Fixes save game screenshots being blank when TAA is disabled.
SlowTimeCameraMovement                  | SSE Engine Fixes           | Fixes camera movement being slow during slow time effects.
TreeReflections                         | SSE Engine Fixes           | Fixes tree LOD reflections. No conflict with ENB.
UnequipAllCrash                         | SSE Engine Fixes           | Fixes a crash when invoking "Actor.UnequipAll" on an actor without an AI process.
VerticalLookSensitivity                 | SSE Engine Fixes           | Makes vertical look sensitivity not tied to framerate.
UnequipAllCrash                         | SSE Engine Fixes           | Fixes a crash when invoking "Actor.UnequipAll" on an actor without an AI process.
WeaponBlockScaling                      | SSE Engine Fixes           | Fixes weapon blocking so it correctly scales off of the blocking actor's weapon.
CleanSKSECosaves                        | SSE Engine Fixes           | Deletes SKSE cosaves with no matching save on launch.
CellInit                                | SSE Engine Fixes           | Fixes a rare crash where a form does not get converted from an id to a pointer.
UseTBBMalloc                            | SSE Engine Fixes           | Replaces standard malloc with tbbmalloc.
FormCaching                             | SSE Engine Fixes           | Caches recently accessed forms. Similar to SSE Fixes.
MaxStdio                                | SSE Engine Fixes           | Raises max file handle limit from 512 to 2048, which should fix "False Save Corruption" bug in most cases.
UseTBBMalloc                            | SSE Engine Fixes           | Replaces standard malloc with tbbmalloc.
SaveAddedSoundCategories                | SSE Engine Fixes           | Saves volume settings for mod-added sound categories to a separate ini file. This functionality is the same as Audio Overhaul for Skyrim SE's dll, but they will not conflict.
TreeLODReferenceCaching                 | SSE Engine Fixes           | Requires FormCaching. Fixes the very slow Tree LOD function that causes framerate drops most noticeable in Riften. Similar to SSE Fixes.
WaterflowAnimation                      | SSE Engine Fixes           | Decouples water flow animation from in-game timescale, so that decreasing/increasing your timescale doesnt mess with the water animation speed.
EnableAchievementsWIthMods              | SSE Engine Fixes           | Enables achievements when you have mods installed.

<div class="datatable-end"></div>




[Unofficial Skyrim Special Edition Patch]: (https://www.nexusmods.com/skyrimspecialedition/mods/266)
[USSEP Changelog]: (https://www.afkmods.com/Unofficial%20Skyrim%20Special%20Edition%20Patch%20Version%20History.html)
[Unofficial Skyrim Creation Club Content Patches]: (https://www.nexusmods.com/skyrimspecialedition/mods/18975)
