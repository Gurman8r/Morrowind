Creatures X
by Pirate Lord

Requires Morrowind, Tribunal and Bloodmoon
--------------------------------------------

Contents:
* Modifies
* Adds Creatures/NPCs
* Adds Eye-Candy Creatures/NPCs
* Adds Ingredients
* Others
* Techie/Advanced Bit

--------------------------------------------

Modifies:
---------
* Virtually all creatures have scripts that improves their stats as the player levels up. Stat change only takes place when they spawn. Script also reduces agility slightly, increasing chance of knock-outs.
* Stronger Dagoth Ur and named Dagoths
* Killing a Dagoth will weaken Dagoth Ur slightly, in a similar way as killing an Ash Vampire
* GMST changes to affect fleeing
* Adjusts Bloodmoon levelled lists to include eye-candy and expands some of the levelled lists so that low level characters get the full effect of the bloodmoon environment.
* New textures for Diseased and Blighted Creatures
* New texture for Old Blue Fin
* Changed the Worm Lord from using the Skeleton mesh to the Liche Mesh
* Creatures have more abilities, to make things slighty more interesting for magicka users.
* Forager and Cliff Racer AI. They start aggressive, but as you kill more and more of them, the less likely that future ones will attack you. Note it's not possible for them to be 100% passive.
* Compatability with Vampire Embrace. NPC creatures will now struggle like guards.
* Compatability with Sixth House Mod. Load Creatures, then Sixth House Mod, and then the Patch esp. Only makes new Sixth House creatures passive to you.
* Compatability with Great House Dagoth Mod. Load Creatures, then Great House Dagoth Mod, and then the Patch esp. Only makes new Sixth House creatures passive to you.


Adds Creatures/NPCs:
--------------------
* Aqua Netch
* Ash Poet
* Blood Wing
* Clannterror
* Clinker
* Daedroth Fiend
* Dark Saint
* Dreughi
* Dreugh Lord
* Famine
* Flame Monarch
* Flaming Skull (removed from levelled lists)
* Frost Monarch
* Ice Worm
* Killer Wasp
* Diseased Kwama Forager
* Diseased Kwama Warrior
* Lost Spirit
* Moose
* Mummy
* Diseased Nix-Hound
* Nix-Pup
* Repair Spider
* Rotworm
* Scarab
* Scorpion
* Giant Scorpion
* Sewer Rat
* Shalk Queen
* Lesser Shalk
* Silver Saint
* Slaughtershark
* Grass Snake
* Ash Snake
* Spider
* Storm Monarch
* Tomb Rat
* Venom Netch Betty
* Venom Netch Bull
* Winged Fiend
* Woodsprite
* Night Stalker
* Land Dreugh
* Centurion Warrior
* Ash Dreamer
* Dreamer Priestess
* Dreamer Priest
* Dreamer Guard
* Dreamer Prophet
* Dreamer Bell Ringer
* Gorgra
* Dremora Overlord
* Armoured Skeletons
* Gorgra Titan
* Horror
* Vampire Hunter
* Werewolf Hunter
* Bandit Gangs
* Parastylus
* Spider Daedra
* Flesh Dremora
* Daedric Bat
* Dreugh Crab
* Kriin (New in 8.5)
* Guardian of Dreams (New in 8.5)
* Tons of "new" Dremora and Daedra and related stuff


Adds Eye-candy Creatures/NPCs:
------------------------------
* Wasp Swarm
* Silver Tail
* Sandcrab
* Sea Horse
* Razor Fish
* Sunheart Fish
* Silver Ridgeback
* Crimson Spinefin
* Gogglefish
* Baby Guar
* Netchling
* Snow Hopper
* Butterfly
* Fast-Foot
* Shalk Herder
* Guar Herder
* Beetles

Adds Ingredients:
-----------------
* Grom
* Wasp Sting
* Scorpion Stinger
* Butterfly Wing
* Snow Hopper Foot
* Silver Tail
* Moose Antler
* Hound Meat, Diseased
* Hound Meat, Blighted
* Alit Meat
* Alit Meat, Diseased
* Alit Meat, Blighted
* Kagouti Meat
* Kagouti Meat, Diseased
* Kagouti Meat, Blighted
* Guar Meat
* Crab Meat, Diseased
* Rat Meat, Diseased
* Rat Meat, Blighted
* Netch Jelly
* Beetle Shell Fragments
* Scrib Shell Fragment
* Parastylus Shell Fragment
* Parastylus Flesh
* Scarab Shell Fragment
* Shalk Shell Fragment
* Daedric Bat Eyeball
* Kriin Meat and Hide

Others:
-------
* Also adds a small handful of new weapons/armor (usually used by the new creatures)
* 6th House Robe
* 6th House Blackend Dream armor
* 6th House Staff

----------------------------------------------------
Techie/Advanced bit
----------------------------------------------------
Installation:
Easiest thing to do is unpack into a seperate folder, and then move/copy the contents into your game folder. In each folder (Sound/Textures/Meshes/Icons) there should be a PLX_CRT folder, which contains everything this mod requires.

Recommended that you create/recreate a Merged Levelled Lists esp. There are programs out there that do this (Such as TESTool and Wyre Mash).
Important! Do not include Creatures if you are creating a Merged Objects file. For some reason, the scripts go really screwy, and a common side effect are massive herds of Guars.


Disable Eye Candy:
Most Eye Candy can be disabled via the console. Useful if your FPS is struggling. Usually this is because of Wasps and Butterflies due to the way they spawn. Every effort has been made to make all scripts and effects as friendly as possible on FPS.

Open the console and change the below variables to 0 to disable, or 1 to enable.
Type: set variablename(below) to 0

plx_crt_show_buts
plx_crt_show_wasps
plx_crt_show_netch
plx_crt_show_fish


Randomised Levelled Stats:
Most creatures that didn't have a script now have a script that randomises their stats.
This is normally a variation of -10% to +10% of the original stat.
So for example if something had a strength of 50, it now has a strength range of 45-55.
Creatures will also level as the player levels up. The difference in level between the creatures level and the players level is added to the % range.
So, if a creature is level 1, and the player is level 11, instead of having a range of -10% to +10%, the range changes to 0% to +20%
This will have a minor impact on the game but at least the challenge increases slightly on older creatures.

Note if you encounter a level 30 creature, and the player is level 30, the stats will be within the -10% to +10% They only improve in relation to the player when the players level is higher then the creatures level.

Randomised stats can be seen in action easily when you encounter swarm creatures such as the Rotworms.


Creature Abilities:
Many creatures have increased natural abilities, this is normally by having a resistance to something, and also a weakness to something. These are using (mostly) the standard spells in the game.
What has been added is determined by the creature type, where it usually appears, and it's ingredients (if it gives some).


Others:
I've removed all changes to vanilla ingredients
Most new ingredients appear in relevant vanilla levelled lists