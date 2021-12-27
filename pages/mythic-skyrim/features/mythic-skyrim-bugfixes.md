---
title: Fixes
summary: Overview of integrated vanilla game bugfixes.
permalink: mythic-skyrim-bugfixes.html
sidebar: mythic-skyrim-sidebar
toc: true
folder: mythic-skyrim
datatable: true
---

<span class="label label-warning">WIP</span>

## Overview

{{ site.skyrim-project }} includes a full collection of vanilla game bugfixes. This page focuses on core gameplay and engine fixes made by USSEP and various SKSE plugins included with {{ site.skyrim-project }}.
- For bugfixes and improvements related to meshes and textures, see [Meshes & Textures](mythic-skyrim-textures.html).
- For UI improvements and fixes, see [User Interface](mythic-skyrim-ui.html).  


## USSEP

[Unofficial Skyrim Special Edition Patch] (USSEP) fixes hundreds of gameplay, quest, NPC, object, item, text and placement bugs with the goal to eventually fix every bug with Skyrim Special Edition not officially resolved by the developers to the limits of the Creation Kit and community-developed tools. Click this link to view the updated and complete [USSEP Changelog].

[Unofficial Skyrim Creation Club Content Patches] (USCCCP) is a bundle of patches to fix the bugs in the Skyrim Creation Club content as well as resolve conflicts between Creation Club mods and USSEP.

{{ site.skyrim-project }} integrates and supports all Creation Club content. Care was taken to ensure other mods integrated into the modlist remained USSEP compatible.

It is important to note that USSEP does not make any fixes that would require SKSE. For fixes that require SKSE, consult the table below.


## SKSE Fixes

The [Skyrim Script Extender] (SKSE) is a tool used by many Skyrim mods that expands scripting capabilities and adds additional functionality to the game. There are many bugs in the vanilla game that require SKSE to be resolved.

You can search to see which SKSE plugin bugfixes are included with {{ site.skyrim-project }}, as well as the source mod for the fix, in the table below.

The purpose of this table is to ensure there are no redundancies or conflicts with vanilla bugfixes made by SKSE plugins, without needing to cross-reference many mod page descriptions.

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
Queued Ref Crash                        | powerofthree's Tweaks      | Fixes crash with faulty ref loading. This may be caused by mods such as Windhelm Bridge Tweaks.
Map Marker Placement                    | powerofthree's Tweaks      | Allows placing map markers near fast travel destinations when fast travel is disabled.
Enable 'Can't Be Taken Book' Flag       | powerofthree's Tweaks      | Restores 'Can't be taken' book flag functionality. Books can be read but not taken into inventory, if this flag is enabled in book records.
Projectile Range Fix                    | powerofthree's Tweaks      | Adjusts range of projectile fired while moving to maintain consistent lifetime. This is a working implementation of the LE fix found here.
CombatToNormal Dialogue Fix             | powerofthree's Tweaks      | Fixes bug where LostToNormal dialogue triggers in place of CombatToNormal, ie. combat ends and NPCs say "must have scared them off".
Cast Added Spells on Load               | powerofthree's Tweaks      | Fixes issue where added spells are dispelled and not reapplied on NPCs upon loading.
Cast No Death Dispel Spells on Load     | powerofthree's Tweaks      | No-death-dispel flagged spells are reapplied on dead NPCs upon loading.
IsFurnitureAnimType Fix                 | powerofthree's Tweaks      | Patches IsFurnitureAnimType condition function so it works on furniture references (previously, it only worked on actors currently using said furniture).
Light Attach Crash                      | powerofthree's Tweaks      | Fixes crash when lights (torches, magelight, quicklight, etc) get attached to unloaded actors.
No Conjuration Spell Absorb             | powerofthree's Tweaks      | Adds NoAbsorb flag to all conjuration spells missing this flag.
GetEquipped Fix                         | powerofthree's Tweaks      | Patches GetEquipped console/condition function so it works with left hand equipped items.
EffectShader Z-Buffer Fix               | powerofthree's Tweaks      | Fixes effectshader z-buffer rendering so particles can show through objects (for non detect-life shaders).
ToggleCollision Fix                     | powerofthree's Tweaks      | Patches ToggleCollision console command to toggle object collision for selected console references.
Load EditorIDs                          | powerofthree's Tweaks      | Loads editorIDs for skipped forms.  EditorIDs can now be used in console commands (player.placeatme dlc1serana). Required for future SPID versions.

<div class="datatable-end"></div>




[Unofficial Skyrim Special Edition Patch]: (https://www.nexusmods.com/skyrimspecialedition/mods/266)
[USSEP Changelog]: (https://www.afkmods.com/Unofficial%20Skyrim%20Special%20Edition%20Patch%20Version%20History.html)
[Unofficial Skyrim Creation Club Content Patches]: (https://www.nexusmods.com/skyrimspecialedition/mods/18975)
[Skyrim Script Extender]: (https://skse.silverlock.org/)

