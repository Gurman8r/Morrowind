***************************************************************** 

The Elder Scrolls III
MORROWIND 

The Madd Leveler 1.0b
http://www.cosmicspeck.com/maddleveler/

***************************************************************** 

Index: 

1. Introduction
2. Description
3. Revision History
4. Installing the Plugin
5. Playing the Plugin 
6. Save Games 
7. Credits and Thanks 
8. Contact Us 
9. Modder/Debugger Notes

***************************************************************** 

1. INTRODUCTION

***************************************************************** 

(NOTE: This mod requires Bloodmoon)

How many times have you started a new game of Morrowind, only to think to yourself, "Oh crap, I have to build up my skill X to go along with my skill Y so I can get a 5x multiplier for Stat Z."  If you're like us and hate planning this stuff out and just want to play the darn game already, this mod is for you. What the Madd Leveler mod does is strip out any need to plan your character out in advance.  Your statistics will increase automatically as you use your skills, and you won't need to worry about trying to obtain 5x multipliers for leveling up.

This mod is also a skill and attribute uncapper, effectively removing the 100 point limit.

IMPORTANT:  Make sure you have read this entire readme before installing this mod, as it makes significant changes to the game!


***************************************************************** 

2. DESCRIPTION

***************************************************************** 

This mod contains several different esp files that alter the standard leveling system used by morrowind. The script used in the mod is fairly well commented and any modifications can be easily made through the Morrowind TESC (see the included guide for details).


ALL PLUGINS REQUIRE THE MADD LEVELER - BASE.ESP TO BE INSTALLED AND LOADED FIRST!  The actual order of the plugins after that doesn't matter, as long as you pay attention to the notes below.


ESP Descriptions:

Madd Leveler - Base.esp

-- Sets all the level up bonus abilities to x1 (rather than x5), regardless of skill point gains
-- Adds an ability point every 3 skill points (to balance above) 
-- Adds 2 spells to your spellbook (see below)
-- Required for the other esps to function properly



Madd Leveler - Cap Remover.esp

-- Changes caps for skills and attributes.  New cap is 1000 :)  You can change the cap for individual skills/attributes using the guide (Note: Maximum value is 4095).



Madd Leveler - Madd Caps.esp  (SAMPLE)

-- This is a sample esp, to show you how easy it is to customize the scripts.  Feel free to use it and/or edit it using the guide.
-- Changes caps for skills and attributes.  New cap is 4000 for most, 1000 for strength, 200 for speed, athletics and acrobatics.

NOTE: The game will use this esp or the Cap Remover.esp, depending on which is loaded last



Madd Leveler - Spell Effects.esp

-- Displays the nice blue fortifying spell effects (as in the pre-1.0 versions) when your stats/skills increase over 100
-- Will not impact framerates like the pre-1.0 effects did (it only displays one effect, not one for each fortification)



Madd Leveler - Madd Health.esp  (SAMPLE)

-- This is a sample esp, to show you how easy it is to customize the scripts.  Feel free to use it and/or edit it using the guide.
-- Adds 5 health points for every endurance point you gain as you increase your stats (outside of the level up screen)
-- Health is in addition to normal level up health gain



Madd Leveler - Sederien Skills.esp

-- Adds an ability point every 4 skill points
-- The base attributes of these skills have been changed:
	Spear - Endurance -> Strength
	Acrobatics - Strength -> Speed
	Conjuration - Intelligence -> Willpower			
	Block - Agility -> Endurance			
	Destruction - Willpower -> Intelligence
	Long Blade - Strength -> Agility 			

NOTE: This esp will NOT work with the default Cap Remover esp, because of the one ability point per every four skill points feature.  If you want to uncap this esp, please edit it as described in the guide.



Madd Leveler - Madd Skills.esp

-- The base attributes of these skills have been changed:
	Spear - Endurance -> Strength
	Acrobatics - Strength -> Speed
	Light Armor - Agility -> Endurance			
	Unarmored - Speed -> Endurance			
	Short Blade - Speed -> Agility
-- Adds one point of luck every 30 skill levels (or 1 per 3 levels) (because I always forget at level up ;)

NOTE:  Please choose either the Madd Skills, Sederien Skills, or neither to install, because the Madd and Sederien skill esps conflict as they both alter the same script.



Madd Leveler - Quest Cap Remover.esp

-- Removes stat/skill caps from quests which reward you by using the Player->ModStat/Skill commands



Madd Leveler - Vampire Cap Remover.esp

-- Allows Vampire characters to continue increasing their stats and skills over 100 by using spells for their extra attributes and skills instead of abilities

IMPORTANT:  I recommend installing the Madd Leveler and this esp BEFORE you become a vampire, but it should work if you are one already.



Madd Leveler - Werewolf Cap Remover.esp

-- Starts applying bonuses to Werewolf once your skills hit 50 (similar to Cortex's Werewolf Evolution mod)
-- Boosts Werewolf stats & skills - Any stats/skills you have that are over 100, and that are not normally reduced to one point when you become a werewolf, have their over 100 values added to your werewolf stats.  (eg:  Human base strength = 150, Werewolf strength = regular werewolf strength + 50)

Note:  It will take a few seconds to get up to full strength when you change into a werewolf, and likewise it will take a couple seconds to regain your abilities after you change back.  This is because of the way werewolf changing is coded into the game.



Madd Leveler - Assassin's Armory Fix.esp

-- Makes the Madd Leveler compatible with Assassin's Armory 7.1 (both mods are required)



Madd Leveler - Illuminated Order Fix.esp

-- Makes the Madd Leveler compatible with Illuminated Order 1.0C

KNOWN ISSUE: Do NOT reset/restart the madd leveler when you have any of the following powers active:
	-Mehrunes Dagon's Blessing
	-Sheogorath's Blessing
	-Pearl's Legacy

I didn't find an easy way to detect them for the reset/restart to add/replace them properly.



Madd Leveler - Lichcraft Fix.esp  (Lichcraft ONLY)

-- Makes the Madd Leveler compatible with Lichcraft 1.0.  



KNOWN ISSUE:  Level one liches have skills fortified by one point.  This may cause your stats to increase as well due to the skill point-based attribute increase. 



Madd Leveler - Illuminated Order And Lichcraft Fix.esp

-- Makes the Madd Leveler compatible with Illuminated Order 1.0C and Lichcraft 1.0 when they are used together
-- Use in addition to the IO and Lichcraft Fixes above



KNOWN ISSUE:  Same as lichcraft.

ONE MORE THING:  These plugins will work best if you install the ML and fixes before you become a lich.  Weird things may happen to your stats otherwise.



There are three new spells in your spellbook:

1) "ML Report": Just a really quick way to check the base stat values as tracked by the mod.  Messageboxes will be display the values of the base stats.

When to use it:
	-- If you think your stats might be screwed up

2) "ML Reset": Resets all your stats back to the internally stored base values (Make sure to remove all fortifications before doing this or they will not get counted after your stats are calculated, and you'll end up with damaged stats.)

When to use it:
	--If your stats/skills get screwed up

3) "ML Restart": Changes all the base stat values to the current stat values, and then runs the reset (Make sure to remove all fortifications before doing this or they will get added to your permanent stats.)

When to use it:

	--When you've cheated using player->setstat/skill
	--When you first start the madd leveler on a character with stats/skills >= 100
	--If another mod gives you a fortify ability on your stats/skills or uses the player->mod/set functions to change your stats/skills
	--If your stats/skills ever get royally screwed up

Ideally, you shouldn't need to use either.  But they should help resolve conflicts with other mods that I haven't tracked down yet.  MAKE SURE YOU SAVE YOUR GAME FIRST BEFORE YOU CAST EITHER OF THESE SPELLS, just in case.  These spells may change your stats in ways you didn't predict.  Try using the reset spell first, as it's less destructive.  If your stats go really screwy, use the player->setstat/skill to fix them and cast the restart spell.  

I also put 100 point sanctuary on the Reset and Restart spells for two seconds, in case you accidentally cast one during combat... By the way... Don't cast these spells in combat ;)



***************************************************************** 

3. REVISION HISTORY

***************************************************************** 

Revision History:

1.0b

-- Atronach fix - Deleted wombburn spell reference from ML - Base.esp

1.0a

-- Fixed fortify spell effects looping with Assassin's Armory fix
-- Fixed AA scripts so you can now check your spell effects as normal

1.0

-- Converted all the spells to curses, with the following effects:
	-enhanced compatibility with spell absorption abilities & atronach sign (no more deactivation of ability)
	-reduced the framerate hit if many stats/skills over 100 are re-applied, thanks to no spell animations
	-curses are re-applied automatically after a remove curse spell, as the spells were after a dispel spell in previous versions
-- Fixed Sederien skills so it uses 4 points to increase stats instead of 3
-- Pause reset/restart script when in menu mode
-- Added a couple scripting sample esps 
-- Added "ML Report" spell to return base stat values as stored by the mod
-- Added the option to view the spell effects for stats increasing over 100
-- Finally added summary text to the esps :P
-- Added compatability fixes for Illuminated Order and Lichcraft

0.9b

-- Fixed a typo that made the game freeze on levelling/resting

0.9

-- Modularized esp files to give players more flexibility (and me less code to duplicate ;) )
-- Added Assassin's Armory Fix
-- Added Uncappers for: Vampires, Werewolves and Quests (oh my!)
-- Added script to provide functional equivalent of the Player->ModStat/Skill commands
-- Rewrote the Reset Script - now two scripts: Reset & Restart
-- Added spells to trigger reset and restart instead of console commands
-- Made it _way_ easier to customize maximum values for individual stats/skills
-- Many other little fixes I can't remember...

0.8b

-- Changed atronach ability so player doesn't lose it when mod is removed

0.8

-- Starting a new game no longer doubles base stats
-- Skills are reduced properly for jail time
-- Attributes and skills are now spells with 9999999... duration
-- Attributes are not capped at 100 at the level up screen
-- Spell absorption / atronach sign accounted for
-- Spells are recast if/when dispelled


0.7

-- Uncapped skills (yay 8^D )
-- Fixed error in base stat/skill calculation - this should fix most fortifying bugs
-- Fixed yet another fortify bug
-- Slowed down luck gain in Madd Version to once per 30 skill levels
-- Capped everything at 1000 instead of 4000
-- Added a (really) quick (and dirty) guide to the scripts

0.6b

-- Added a fourth esp
-- Altered standard & no caps versions so that skills are left with default attributes

0.6

-- Fixed a fortify bug on stats > 100
-- Changed attributes over 100 to be fortifications instead of forcing players to remove attribute fortifications/drains before seeing an attribute increase 
-- Added a third esp

0.5

-- Fixed another fortify bug -- for stats

0.4

-- Fixed the fortify bug -- for skills

0.3

-- Added additional version of esp
-- Added this nice readme ;)

0.2b 

-- Fixed fortifying bug 
-- Restored skill gain rate to normal 

0.2 Internal release

0.1 Initial release


***************************************************************** 

4. INSTALLING THE PLUGIN 

***************************************************************** 

To install the plugin, unzip the esp files into your Morrowind Data Files directory.  *IMPORTANT* This mod requires Bloodmoon!


***************************************************************** 

5. PLAYING THE PLUGIN 

***************************************************************** 

Simply check which plug-ins you want to use (see above for descriptions) and start the game as usual. 


When starting a new game:

When you talk to Sellus Gravius for the first time (when it tells you not to use persuasion on him), you will see a message that says "Madd Leveler Enabled".  This mod is active from then on.





UPGRADING FROM 0.9+ VERSIONS:

Copy the esps over the existing esps in your data files directory.

Start the game as usual.






UPGRADING FROM PRE-0.9 VERSIONS:

BEFORE YOU INSTALL this mod, remove all your drains/fortifications/etc from you character and SAVE the game (and back it up too).  Version 0.9 switches the looping routine over to a new script and the madd leveler will automatically reset for existing users.

Delete all the old versions of the Madd leveler esps from data files directory (just in case :P).

Finally, either cast the "ML Restart" spell or type "StartScript Madd_Leveler_Restart" in the console to make sure everything is set up right.





EXISTING GAMES / QUICK STARTS:

If you are adding this mod to an existing game or using a quick start mod, perform these steps to make sure that the new version is working properly:

1) Remove all drains/fortifications/etc from your character
2) Open console, type:  StartScript Madd_Leveler (<-- Note this has changed since 0.8b)

And you should be good to go...





PORTING OVER FROM MEPHISTO'S CAP REMOVER (Or if you have cheated and BUMPED your stats really high):

0) Make sure you have removed mephisto's cap remover.
1) Remove all drains/fortifications/etc from your character
2) Open console, type:  StartScript Madd_Leveler 

Next, pick one:

3A) At console, type: StartScript Madd_Levler_Restart
3B) Cast "ML Restart" from your spellbook.





Increasing Stats/Skills (Cap Remover active):

When your skills/stats increase with caps removed, they will increase normally up to 99.  Once they reach 100, fortify spells will be cast on your character to increase them further.  They will then be bumped back to 99 so they can keep increasing normally.

For example:
	Mylon increases his long blade skill to 99.  Nothing new here.
	Mylon increases his skill to 100.  His skill is bumped back down to 99, and he is fortified for one point of long blade.
	Mylon increases his skill to 101.  His skill is bumped back down to 99, and he is fortified for two points of long blade.
	And so on...

If your stats/skills go to 100, and no fortifications are present, you won't be able to continue increasing them... And this would be a bug.  I have _never_ seen this happen, but if you do see it, here's what you can do:  

You should have a spell in your spellbook called "ML Reset".  Cast it.  It will reset all your stats and skills to the internal base values.

OR, you can do it the long way:

Type this in the console:

StartScript Madd_Leveler_Reset






Leveling Up (Caps Removed):

When you level up and one or more of your stats are above 100, the level up screen will show those stats as being 99.  This is normal; it is to allow you to continue to increase your stats above 100.






Important note for Vampires:

I recommend installing the Madd Leveler and the vampire cap remover BEFORE you become a vampire.  It will work if you're one already, but you may find your bonuses doubled :P






Potential Incompatibilities:

This mod should *not* be incompatible with any other mods that affect the rate at which skills increase, etc. The only incompatibilities may be mods which change the attributes that skills are tied to... But you can edit this script in the TES:CS.

This mod may also not function properly if used in conjunction with other mods which alter the player's attributes/skills using the Set and Mod functions, such as other leveling mods.  This is because the mod uses a base value calculation which attempts to avoid any fortification/drain issues while at the same time being clean and unobtrusive.  This shouldn't be a major issue, as most mods that use these functions on the player serve purposes similar to this mod.  


Known Incompatibilities:

Mephisto's Cap Remover (also removes caps)
Assassin's Armory 7.1 - fix provided, also works with 7.0, lower versions not guaranteed compatible
Lichcraft 1.0 - fix provided, lower versions not guaranteed compatible
Illuminated Order 1.0C - fix provided, lower versions not guaranteed compatible
KNOWN ISSUE WITH FIX: Do NOT reset/restart the madd leveler when you have any of the following powers active:
	Mehrunes Dagon's Blessing
	Sheogorath's Blessing
	Pearl's Legacy



I didn't find an easy way to detect them for the reset/restart to add/replace them properly.

***************************************************************** 

6. SAVE GAMES

***************************************************************** 

This should not invalidate your old save games. But making a backup copy is always a good idea... 

If you save your game while this plugin is loaded, you may encounter error messages when you reload the saved game without the plugin. But you will be able to continue on with the original game. 

(Caps Removed)  If you remove the plugin, you will notice that your stats will decrease back to 99 if they were over 100 prior to removal.  This is because all the spells to raise your stats are gone.  


***************************************************************** 

7. CREDITS AND THANKS 

***************************************************************** 

Many people contributed to the creation of this mod and should be recognized for their input: 

Sederien - For the initial request and idea, work on the readme, & of course the Madd Leveler Website!
Madd_Mugsy - scripting/editing
VenomByte - For telling me that curses affect stats like spells
Cortex - For werewolf balancing ideas and scripts
MysticResearcher - Scripting research
Miral007 - For scripting attempts and lessons
Balor - For the original leveling mod which spawned this idea
ppi, alexandrian_librarian, Mylon, Aeroldoth, and all the others from the elder scrolls message boards - For bug testing and general helpful comments :) 

Thanks as well to Bethesda and the Morrowind staff for such a great game! 

Cleaned with TES Advanced Mod Editor (by Erik Benerdal). 

If you'd like to include this script in your mod, by all means do so, but please give credit to the folks above for their hard work and creativity.


***************************************************************** 

8. CONTACT US

***************************************************************** 

Any questions or concerns can be brought to Madd Mugsy at Madd_Mugsy@msn.com, Sederien 
at sederien@cosmicspeck.com, or the Elder Scrolls forums at: 

http://www.elderscrolls.com/ubbthreads/showflat.php?Cat=&Board= 
UBB7&Number=2815983&fpart=&PHPSESSID= 


***************************************************************** 

9. MODDER/DEBUGGER NOTES

***************************************************************** 

If you would like to detect if someone is using the Madd Leveler, you can check the following global variables:

1) Madd Leveler is running:	mlRunOnce > 0

2) Madd Leveler loop state:  
		mlStatus = 0 -- main loop is running
		mlStatus > 0 -- checking & fortifying skills/stats
		mlStatus = -1 -- to put the loop on hold

3) Madd Leveler is resetting:	mlReset > 0

4) Cap Remover is on:	MaxStat < 100 and/or MaxSkill < 100

5) Werewolf is uncapped:	mlUncapWerewolf > 0

6) Vampire is uncapped:		mlUncapVampire > 0

7) Get a Maximum value for a skill/stat:	MaxStrength, MaxLongBlade, etc.

8) Access the player's base stats (exclusive of fortifications and drains):	Base_Strength, Base_Athletics, etc.

9) Find out how many points of fortifications are allocated:  Fort_StrengthMax, Fort_AcrobaticsMax, etc.

10) Find out how many points of fortifications have actually been added: Fort_Strength, Fort_Acrobatics, etc.
	(Note:  #9 and #10 should return the same number, unless the fortifications have been removed somehow)

11) Do the equivalent of a Player->Mod command:
		Set Adj_Strength To 5 <-- increase strength by 5
		Set Adj_Endurance To -2 <-- decrease endurance by 2
		Startscript mlAdjust <-- apply adjustments

12) Remove curse was cast on player:  mlRemoved > 0
	(Note: this variable won't be on for more than a second or so before the loop catches it and restores the fortifications)

13) Spell effects esp is on:  mlShowEffect > 0 


For non-modders who want to check the values of these variables, at the console type:

	Messagebox "%.0f", [VariableName]
	
where [VariableName] can be any of the variables listed above.


Please contact Madd Mugsy if you need any other information :)