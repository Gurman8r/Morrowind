===============================================================================
|                            Expansions Integrated                            |
|                        A Morrowind Mod, Version 1.1.2                       |
|                                by Necrolesian                               |
===============================================================================

---------
Summary |
---------

This mod integrates (much of) the content of the Tribunal and Bloodmoon
expansions within the rest of the game world. Many items and creatures from the
expansions, which could previously be found only in Mournhold or Solstheim, can
now be found throughout Vvardenfell.

Dragon32's Expansion Integration does something very similar, and partly
inspired this mod. This mod makes a number of different decisions than
Dragon32's mod does in terms of which items/creatures to integrate and how to
do so. Use whichever one you like best (though obviously not both).

Much of the item placement in this mod (and all of the creature placement) is
done via leveled lists, though a number of items are handplaced. This mod
incorporates Adamantium Armor Integrated, which handplaces one instance of each
Adamantium armor piece in Vvardenfell, so there's no need to use that mod along
with this one.

The following items and creatures are integrated in one way or another by this
mod:

- Tribunal armor: Adamantium, Dark Brotherhood
- Tribunal weapons: Adamantium (including Adamantium Jinkblade of Wounds),
     Ebony Scimitar (unenchanted)
- Tribunal clothing: Common Pants, Shirt and Shoes
- Tribunal ingredients: All except Adamantium Ore
- Tribunal creatures: Durzog (four types), Centurion Archer (two types),
     Advanced Steam Centurion, Greater Ancestor Ghost, Lich
- Bloodmoon armor: Wolf, Bear, Nordic Mail
- Bloodmoon weapons: Huntsman, Nordic Silver, Berserker (enchanted), Blood Axe,
     Winterwound Dagger
- Bloodmoon clothing: Common Pants, Robe, Shirt and Shoes
- Bloodmoon ingredients: All except Raw Stalhrim, Snow Bear and Snow Wolf Pelt,
     and Wolfsbane Petals
- Bloodmoon drink: Nord Mead
- Bloodmoon creatures: Grizzly Bear, Plague Bear, Tusked Bristleback, Wolf (two
     types), Plague Wolf, Dire Frost Atronach, Bonewolf, Skeleton Berserker
     (two types), Greater Skeleton Champion

A couple of the expansions' creatures have been added at levels lower than when
they can be found in the expansion. For example, War Durzogs can be encountered
at level 20 in Vvardenfell. Users of Tribunal Rebalance and Bloodmoon Rebalance
will have an easier time of this.

Included is an optional Tribunal-only version, for those who don't like the
addition of the Bloodmoon items/creatures. Note that the Tribunal-only version
also omits the fix to the Greater Skeleton Champion and the change to the Blood
Axe enchantment described below.

Also included is a "Fewer BM Creatures" version, which is basically the full
version of the mod with the following creatures omitted: Grizzly Bear, Plague
Bear, Tusked Bristleback, Wolf (both types), Plague Wolf.

The Details section below lists most of the specific changes made by this mod.
See also the "spoilers" document in the archive for a list of locations of
certain items (Adamantium armor and weapons) that have been placed by hand.

---------
Details |
---------

This section will detail the changes made by this mod - exactly which items and
creatures are placed and how. This section contains some spoilers, though the
exact locations of Adamantium armor and weapon pieces are omitted (see the
spoilers document for those).

Tribunal Armor
--------------

- Adamantium Armor: Each piece is handplaced in exactly one spot on
Vvardenfell. See the spoilers document in the archive if you want to know
exactly where. (The locations are the same as in Adamantium Armor Integrated,
so there's no need to use that mod with this one.)

- Dark Brotherhood Armor: Has been given to a number of Dark Brotherhood
members (or likely members) on Vvardenfell, specifically: Severa Magia and
Nidara Herandus in Ald Sotha, and Durus Marius and Sovisa Adas in
Assernerairan. Herandus and Adas have all pieces, while Magia and Marius lack
the helm.

Tribunal Weapons
----------------

- Adamantium Weapons: Each weapon has been handplaced in exactly one spot on
Vvardenfell. This includes the Axe, Claymore, Mace, Shortsword, Spear, and the
Adamantium Jinkblade of Wounds. The spoilers document in the archive lists
their locations.

- Ebony Scimitar: The unenchanted version has been added to the following
leveled lists:

random ebony weapon
random excellent melee weapon (15)
random_golden_saint_weapon

(The number in parentheses is the level the item has been added at. Here and
elsewhere in this document, where a level is not specified, the item has been
added at level 1.)

It's also been handplaced in one location on Vvardenfell: Ghostgate: Tower of
Dusk Lower Level.

The enchanted version (Ebony Scimitar_her) has not been added anywhere.

Tribunal Clothing
-----------------

Tribunal adds two new each of Common Pants, Common Shirt and Common Shoes (the
IDs for each end in 06 and 07). These items have been added to the leveled
lists random_de_pants, random_de_shirt and random_de_shoes_common respectively.

Tribunal's Common Skirts are not added, nor are the expensive clothing items
(due to a lack of appropriate leveled lists to add them to).

Tribunal Ingredients
--------------------

All new ingredients except Adamantium Ore (including Durzog Meat, Golden Sedge
Flowers, Horn Lily Bulb, Lloramor Spines, Meadow Rye, Nirthfly Stalks, Noble
Sedge Flowers, Scrib Cabbage, Sweetpulp and Timsa-Come-By Flowers) have been
added to the leveled lists random_ingredient and random_ingredient_diff.

Scrib Cabbage has also been added to random_de_cheapfood_01_nc, random_de_
cheapfood_01_ne and random_food.

Adamantium Ore has not been added anywhere; it's still exclusive to Mournhold.

Tribunal Creatures
------------------

- Durzog: Four types of Durzogs are placed by this mod: durzog_wild_weaker,
durzog_wild, durzog_diseased and durzog_war. They've been added to the
following leveled lists, at levels 5, 10, 12 and 20 respectively:

ex_azurascoast_lev+0
ex_azurascoast_lev+2
ex_azurascoast_lev-1
ex_azurascoast_sleep
ex_bittercoast_lev+0
ex_bittercoast_lev+2
ex_bittercoast_lev-1
ex_bittercoast_sleep
ex_grazelands_lev+0
ex_grazelands_lev+2
ex_grazelands_lev-1
ex_grazelands_sleep
ex_molagmar_lev+0
ex_molagmar_lev+2
ex_molagmar_lev-1
ex_molagmar_sleep
ex_westgash_lev+0
ex_westgash_lev+2
ex_westgash_lev-1
ex_westgash_sleep
ex_wild_all_lev+0
ex_wild_all_lev+2
ex_wild_all_lev-1
ex_wild_all_sleep
in_cave_all_lev+0
in_cave_all_lev+2
in_cave_all_lev-1

(Note that, here and elsewhere, levels have been adjusted as appropriate for
the lev+x and lev-x lists.)

The special type durzog_war_trained is not included.

- Centurion Archer, Advanced Steam Centurion: There are two types of Centurion
Archer that have been integrated: centurion_projectile and centurion_
projectile_C (the latter is more dangerous because of its enchanted shock
bolts). Only the "regular" type of Advanced Steam Centurion is included.

They've been added to the following leveled lists, at levels 10, 12 and 20
respectively:

in_dwe_all_lev+0
in_dwe_all_lev+2
in_dwe_all_lev-2
in_dwe_cent_lev+0
in_dwe_cent_lev+2
in_dwe_cent_lev-2

- Greater Ancestor Ghost: Has been added to the following leveled lists, at
level 15:

in_tomb_all_lev+0
in_tomb_all_lev+2
in_tomb_all_lev-2

- Lich: Has been added to the following lists, at level 20:

in_tomb_all_lev+0
in_tomb_all_lev+2
in_tomb_all_lev-2
in_tomb_skele_lev+0
in_tomb_skele_lev+2
in_tomb_skele_lev-2

In addition, the "Calculate from all levels <= PC's level" flag has been set
for the above leveled lists, and for the three in_tomb_bone lists. They were
(almost) the only leveled creature lists in the vanilla game without that flag
set. Now there will be much more diversity in tomb undead, rather than always
seeing the same creature all the time.

Bloodmoon Armor
---------------

- Wolf Armor: Each piece has been added to the appropriate l_n_armor lists (for
boots, cuirass, gauntlets, greaves, helmet, pauldrons and shields) at level 3.

In addition, a new leveled list has been created (necro_random_armor_wolf) with
all pieces, and this new list has been added to random_smuggler_1-5 and random_
bandit_1-5.

The enchanted Snow Wolf Armor is not added anywhere.

- Bear Armor: Like with Wolf Armor, each piece has been added to the
appropriate l_n_armor list at level 3. A new list (necro_random_armor_bear) has
been created with all pieces and added to random_smuggler_6-10 and random_
bandit_11+.

The enchanted Snow Bear Armor is not included.

- Nordic Mail Armor: Each piece has been added to the appropriate l_n_armor
list at level 20.

Bloodmoon Weapons
-----------------

- Huntsman Axe: Has been added to l_n_wpn_melee_axe (6) and random_weapon_
melee_basic.

- Huntsman War Axe: Added to l_n_wpn_melee_axe (17).

- Huntsman Longsword: Added to l_n_wpn_melee_long blade (5) and random_weapon_
melee_basic.

- Huntsman Spear: Added to l_n_wpn_melee_spear (5) and random_weapon_melee_
basic.

- Huntsman Crossbow: Added to l_n_wpn_missile_xbow (10) and random_weapon_
melee_basic. (It's not a melee weapon, but the Steel Crossbow is already on the
latter list in vanilla.)

- Huntsman Bolt: Added to l_n_wpn_missile_bolt (7).

- Nordic Silver Axe, Battleaxe: Added to the following leveled lists:

l_n_wpn_melee_axe (18, 20)
random excellent melee weapon (14, 15)
random_nordic_weapons (13, 15)

- Nordic Silver Mace: Added to l_n_wpn_melee_blunt (15) and random excellent
melee weapon (10).

- Nordic Silver Longsword: Added to l_n_wpn_melee_long blade (12) and random
excellent melee weapon (12).

- Nordic Silver Claymore: Added to the following lists:

l_n_wpn_melee_long blade (17)
random excellent melee weapon (15)
random_nordic_weapons (14)

- Nordic Silver Dagger, Shortsword: Added to l_n_wpn_melee_short blade (12, 13)
and random excellent melee weapon (7, 8).

- Berserker Silver Axe, Battleaxe: These enchanted weapons have been added to
l_m_wpn_melee_axe (15, 18).

- Berserker Silver Longsword, Claymore: Added to l_m_wpn_melee_long blade (9,
20).

- Blood Axe: This one is unique in that the weapon's enchantment has also been
edited. In vanilla, this weapon's enchantment includes Damage Strength 4 points
for 30 seconds, for 120 points total Damage Strength. This is insane. The
enchantment "bm bloodaxe" has been changed from Damage Strength to Absorb
Strength instead.

The weapon (with new, less insane enchantment) has been added to the leveled
list l_m_wpn_melee_axe (14).

- Winterwound Dagger: Added to l_m_wpn_melee_short blade (20).

Bloodmoon Clothing
------------------

Bloodmoon adds four each of Common Pants, Common Shirts and Common Shoes, and
two Common Robes. These items have been added to the lists random_de_pants,
random_de_shirt, random_de_shoes_common and random_de_robe respectively.

Bloodmoon's Common Gloves are not added anywhere.

Bloodmoon Ingredients
---------------------

The ingredients Bear Pelt, Bristleback Leather, Holly Berries, Ripened and
Unripened Belladonna Berries and Wolf Pelt have been added to the leveled lists
random_ingredient and random_ingredient_diff.

Grahl Eyeball, Gravetar, Heartwood and Horker Tusk have been handled a bit
differently. All are from creatures that have not been placed in Vvardenfell,
and so should be rarer. They've been added to random_ingredient_diff, but not
to random_ingredient directly.

Instead, a new list has been created (necro_random_ingred_bm_rare, chance none
50) with all four ingredients, and this new list has been added to random_
ingredient. This way, there's only one chance each calculation for one of the
rare ingredients, and even if the rare list is selected, there's still a 50%
chance of nothing.

Raw Stalhrim, Snow Bear and Snow Wolf pelts, and Wolfsbane Petals are not added
anywhere; they're still exclusive to Solstheim.

Bloodmoon Drink
---------------

- Nord Mead: This one is handled somewhat similarly to the rare Bloodmoon
ingredients. It's not added to leveled lists directly. Instead, the vanilla
leveled list random_drinks_nord (which contains four other beverages in
addition to mead) is itself added to random_drinks_01 and random_alchemy_diff.
This way, Nord Mead will be substantially rarer than other beverages on
Vvardenfell, but you'll still come across it once in a while.

In addition, mugs have been handplaced in two locations in Dagon Fel: End of
the World Renter Rooms and Andre Maul's Tower.

Bloodmoon Creatures
-------------------

- Grizzly Bear: Has been added to the following leveled lists, at level 7:

ex_ascadianisles_lev+0
ex_ascadianisles_lev+2
ex_ascadianisles_lev-1
ex_ascadianisles_sleep
ex_grazelands_lev+0
ex_grazelands_lev+2
ex_grazelands_lev-1
ex_grazelands_sleep
ex_westgash_lev+0
ex_westgash_lev+2
ex_westgash_lev-1
ex_westgash_sleep
ex_wild_all_lev+0
ex_wild_all_lev+2
ex_wild_all_lev-1
ex_wild_all_sleep
in_cave_all_lev+0
in_cave_all_lev+2
in_cave_all_lev-1

- Plague Bear: Added to the following lists, at level 10:

ex_sheogorad_lev+0
ex_sheogorad_lev+2
ex_sheogorad_lev-1
ex_sheogorad_sleep
ex_westgash_lev+0
ex_westgash_lev+2
ex_westgash_lev-1
ex_westgash_sleep
ex_wild_all_lev+0
ex_wild_all_lev+2
ex_wild_all_lev-1
ex_wild_all_sleep

- Tusked Bristleback: Added to the following lists, at level 12:

ex_ascadianisles_lev+0
ex_ascadianisles_lev+2
ex_ascadianisles_lev-1
ex_ascadianisles_sleep
ex_grazelands_lev+0
ex_grazelands_lev+2
ex_grazelands_lev-1
ex_grazelands_sleep
ex_sheogorad_lev+0
ex_sheogorad_lev+2
ex_sheogorad_lev-1
ex_sheogorad_sleep
ex_wild_all_lev+0
ex_wild_all_lev+2
ex_wild_all_lev-1
ex_wild_all_sleep
in_cave_all_lev+0
in_cave_all_lev+2
in_cave_all_lev-1

- Wolf: Two types of wolves are added by this mod: bm_wolf_grey_lvl_1 and bm_
wolf_grey. They've been added to the following leveled lists, at levels 3 and 7
respectively:

ex_ascadianisles_lev+0
ex_ascadianisles_lev+2
ex_ascadianisles_lev-1
ex_ascadianisles_sleep
ex_azurascoast_lev+0
ex_azurascoast_lev+2
ex_azurascoast_lev-1
ex_azurascoast_sleep
ex_grazelands_lev+0
ex_grazelands_lev+2
ex_grazelands_lev-1
ex_grazelands_sleep
ex_molagmar_lev+0
ex_molagmar_lev+2
ex_molagmar_lev-1
ex_molagmar_sleep
ex_sheogorad_lev+0
ex_sheogorad_lev+2
ex_sheogorad_lev-1
ex_sheogorad_sleep
ex_westgash_lev+0
ex_westgash_lev+2
ex_westgash_lev-1
ex_westgash_sleep
ex_wild_all_lev+0
ex_wild_all_lev+2
ex_wild_all_lev-1
ex_wild_all_sleep
in_cave_all_lev+0
in_cave_all_lev+2
in_cave_all_lev-1

- Plague Wolf: Added to the following lists, at level 8:

ex_grazelands_lev+0
ex_grazelands_lev+2
ex_grazelands_lev-1
ex_grazelands_sleep
ex_sheogorad_lev+0
ex_sheogorad_lev+2
ex_sheogorad_lev-1
ex_sheogorad_sleep
ex_westgash_lev+0
ex_westgash_lev+2
ex_westgash_lev-1
ex_westgash_sleep
ex_wild_all_lev+0
ex_wild_all_lev+2
ex_wild_all_lev-1
ex_wild_all_sleep

- Dire Frost Atronach: This one required special handling. This creature
(atronach_frost_bm) is placed in vanilla only in Aesliip's Lair, with a script
attached associated with the related quest. The script can't be removed without
breaking (one path of) that quest, and it would cause problems if attached to
creatures anywhere else.

So, a copy of this creature has been created (necro_atronach_frost_bm). The
script has been removed from the new creature, and it's been added to the
following lists at level 15:

in_dae_all_lev+0
in_dae_all_lev+2
in_dae_all_lev-2
in_dae_atronach_lev+0
in_dae_atronach_lev+2
in_dae_atronach_lev-2

and the following lists at level 18:

ex_molagmar_lev+0
ex_molagmar_lev+2
ex_molagmar_lev-1
ex_molagmar_sleep

The original creature remains unmodified and exclusive to Aesliip's Lair.

- Bonewolf: Added to the following lists, at level 5:

in_tomb_all_lev+0
in_tomb_all_lev+2
in_tomb_all_lev-2
in_tomb_all_lev_trib
in_tomb_bone_lev+0
in_tomb_bone_lev+2
in_tomb_bone_lev-2

It was added to the in_tomb_bone lists and not the in_tomb_skele lists because
otherwise the in_tomb_bone lists would have remained unchanged, and the
Bonewolf is the most appropriate creature to add to them.

Also, the addition to in_tomb_all_lev_trib will diversify the undead in
Mournhold. (Skeleton Berserkers and Greater Skeleton Champions below are also
added to this list.)

- Skeleton Berserker: There are two creatures added here, skeleton nord and
skeleton nord_2, which are very similar except the _2 variant has more health.
They've been added to the following leveled lists, at levels 9 and 10
respectively:

in_tomb_all_lev+0
in_tomb_all_lev+2
in_tomb_all_lev-2
in_tomb_all_lev_trib
in_tomb_skele_lev+0
in_tomb_skele_lev+2
in_tomb_skele_lev-2

- Greater Skeleton Champion: This one also required some special handling.

There are actually three different types of this creature. The creatures bm_sk_
champ_bloodskal01 and 02 are placed only in Bloodskal Barrow, and have a script
attached to them which disables them until you pick up the sword in that
barrow.

The third type, bm skeleton champion gr, is not in Bloodskal Barrow, but
instead just on a few generic Bloodmoon leveled creature lists. However, it
also has the bloodskal script attached to it, which causes all instances of
this creature to not appear until the sword in Bloodskal Barrow has been
picked up.

Since this is clearly a mistake, the script has been removed from bm skeleton
champion gr. This creature, now that it will actually show up as intended, has
been added to the following lists at level 15:

in_tomb_all_lev+0
in_tomb_all_lev+2
in_tomb_all_lev-2
in_tomb_all_lev_trib
in_tomb_skele_lev+0
in_tomb_skele_lev+2
in_tomb_skele_lev-2

--------------
Installation |
--------------

Use a mod management tool such as Wrye Mash, or just copy the plugin of your
choice to your Data Files directory and select it in the Morrowind Launcher.
Use only one of the included plugins.

-----------------
Version History |
-----------------

Version 1.1.2 - 2021-01-19
   - Added "Fewer BM Creatures" version omitting the more conventional
        Bloodmoon creatures such as bears and wolves.

Version 1.1.1 - 2020-10-27
   - Incorporated Patch for Purists fixes for Hrordis, Durus Marius and Severa
        Magia (now in Dark Brotherhood faction).

Version 1.1 - 2020-04-23
   - Added optional Tribunal-only version.
   - Removed Greater Ancestor Ghost from in_tomb_skele lists.

Version 1.0 - 2020-04-21
   - Initial release.

---------
Contact |
---------

Feel free to contact me on the Nexus with any comments or suggestions. You can
also find me on Discord as Necrolesian#9692, or you can email me at
necrolesian@riseup.net.

-------
Usage |
-------

You can use this however you want.