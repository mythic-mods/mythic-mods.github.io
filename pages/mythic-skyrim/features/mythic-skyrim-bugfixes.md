---
title: Fixes
summary: Overview of some vanilla game bugfixes integrated with Mythic Skyrim.
permalink: mythic-skyrim-bugfixes.html
sidebar: mythic-skyrim-sidebar
toc: true
folder: mythic-skyrim
datatable: true
---



You can search to see if a particular bug from the vanilla game has been addressed in the search bar below.

<div class="datatable-begin"></div>

Name    						        | Mod               | Description
--------------------------------------- | ----------------- | -----------
Actor Value Percentage	                | Scrambled Bugs    | Fixes incorrect values being displayed in the HUD for player and NPC actor values (health, stamina, etc.) due to the target having any temporary buffs or debuffs to the relevant actor value.
Apply Spell Perk Entry Points: Arrows   | Scrambled Bugs    | Fixes the Bullseye perk from incorrectly applying
Harvested Flags                         | Scrambled Bugs    | Fixes flora and trees that have respawned in a loaded from being incorrectly harvested once again. This is an alternative to the Flora Respawn Fix.
Hit Effect Race Condition               | Scrambled Bugs    | Fixes race condition from preventing hit effects being applied to an actor if their mesh loads after a magic effect is first updated.
Magic Effect Conditions                 | Scrambled Bugs    | Fixes a floating-point error that will gradually prevent the conditions of magic effects from being updated. The longer a magic effect has been running for, the more frequently this will occur (article﻿). This is an alternative to the ability condition fix in Bug Fixes SSE.
Magic Effect Flags                      | Scrambled Bugs    | Fixes magic effects not respecting their flags when scaling their duration and magnitude.
Mod Armor Weight Perk Entry Point       | Scrambled Bugs    | Fixes the Mod Armor Weight perk entry point from not modifying the weight of just the armor you are wearing, but incorrectly modifying the weight of stacks of that armor.
Quick Shot                              | Scrambled Bugs    | Fixes the Quick Shot perk not being accounted for when calculating the power of an arrow fired by the player.
Terrain Decals                          | Scrambled Bugs    | Fixes decals not being applied to the terrain in cells that have been partially unloaded.
Training Menu Text                      | Scrambled Bugs    | Fixes the cost of a lesson displayed in the training menu not being affected by any buffs or debuffs to the relevant skill.
Weapon Charge                           | Scrambled Bugs    | Fixes the charge of equipped enchanted weapons only being restored to the charge they were when last equipped or recharged.

<div class="datatable-end"></div>
