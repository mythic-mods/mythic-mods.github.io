---
title: Mesh & Texture Fixes
summary: Overview of vanilla mesh and texture fixes integrated with Mythic Skyrim.
permalink: mythic-skyrim-mesh-fixes.html
sidebar: mythic-skyrim-sidebar
toc: true
folder: mythic-skyrim
---

## Mesh & Texture Fixes

<button type="button" class="btn btn-info" data-toggle="collapse" data-target="#demo">Weapons Armor Clothing and Clutter Fixes</button>
<div id="demo" class="collapse">
  
  - Corrects many of the bugs found in the vanilla weapon, armor, clothing, jewelry, and clutter records.
  - Improves consistency and balance between different items (value, weight, damage, keywords, etc).
  - Weapons and armor will scale in a predictable and consistent manner.
  - The strength of an enchantment on a piece of enchanted jewelry is now properly reflected by the quality of the base jewelry.
  
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title">
        <a data-toggle="collapse" href="#collapse1">Weapons Armor Clothing and Clutter Fixes</a>
      </h4>
    </div>
    <div id="collapse1" class="panel-collapse collapse">
      <ul class="list-group">
        <li class="list-group-item">Corrects many of the bugs found in the vanilla weapon, armor, clothing, jewelry, and clutter records.</li>
        <li class="list-group-item">Improves consistency and balance between different items (value, weight, damage, keywords, etc).</li>
        <li class="list-group-item">Weapons and armor will scale in a predictable and consistent manner.</li>
        <li class="list-group-item">The strength of an enchantment on a piece of enchanted jewelry is now properly reflected by the quality of the base jewelry.</li>
        <li class="list-group-item">Perks that didn't apply consistently to all items in the game have been fixed.</li>
        <li class="list-group-item">Female clothing variants will now use the correct texture in first-person.</li>
        <li class="list-group-item">Changes the crafting categories to help organize and declutter the crafting menus.</li>
        <li class="list-group-item">Increases the speed of arrows and bolts by 50% and makes them fly at a slightly flatter trajectory.</li>
        <li class="list-group-item">Changes the stats and keywords for the dragon priest masks to better balance them with other gameplay options.</li>
        <li class="list-group-item">Adjusts the stats of Dwarven, Elven, and Orcish weapons to make them consistent with the rank and quality of their respective armors and the progression of the Smithing perks.</li>
        <li class="list-group-item">Switches the values and stats of Daedric and Dragonbone weapons, so that Daedric are the more powerful.</li>
        <li class="list-group-item">Some previously unplayable or inaccessible items are now playable and/or accessible in game.</li>
        <li class="list-group-item">Allows circlets to be worn with hoods.</li>
        <li class="list-group-item">Almost all instances of hooded robes have been removed from the game and replaced with separate robe and hood combinations.</li>
        <li class="list-group-item">Adjusts the loot found in certain furniture containers to be consistent with both the class and the type of furniture.</li>
        <li class="list-group-item">Certain items have been renamed for easier sorting or to better fit the in-game appearance of that item.</li>
        <li class="list-group-item">Necklaces and/or rings that were invisible when worn with certain clothing can now be seen.</li>
        <li class="list-group-item">Potion bottles will now use the correct meshes, and Poison bottles will no longer appear flat and dull.</li>
      </ul>
    </div>
  </div>
</div>


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
