~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
       Fish With Fishing Poles (by RacerPlume/Ian)
             Skill Exposer / Expansion v2.1
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Expansion by Booze (B00ze64) 2021-08

	B00ze64@zoho.com (best)
	B00ze64@hotmail.com (if you must)
	Note that hotmail spam filters suck mail like a blackhole...

Fish With Fishing Poles: https://www.nexusmods.com/morrowind/mods/47230
Merlord's Skills Module: https://www.nexusmods.com/morrowind/mods/46034

This is a small ESP file that loads AFTER RacerPlume's Fishing.esp, and a MWSE
script that together, aim to make Pole Fishing more useful as a source of food
for Ashfall. This Expansion also makes the Pole Fishing skill visible, and ties
it to Endurance, which should make leveling that stat easier (same as Survival
skill in Ashfall). You obviously need the original Fish With Fishing Poles mod,
as this here only expands on it.

Everything in this package is optional, but you do need Merlord's Skill Module
installed if you want to see the Pole Fishing skill in the Other Skills section
of your character. And if the ONLY thing you want is to see your Pole Fishing
skill, then simply do not load the Fishing-Expansion.esp module.

If all you want is to display your skill then all you'll want out of this
Expansion is the Skills module (i.e. do NOT load the Fishing-Expansion.esp).
Please also see RacerPlume's other Survival/Crafting mods:

https://www.nexusmods.com/morrowind/users/64066421?tab=user+files

Changes made when Merlord's Skill module is installed and when you also load
Fishing-Expansion.esp ->

- Increased chance to catch fish (+ 10%).
- Pole Fishing skill is visible and tied to Endurance.
- You freeze for 3 seconds instead of 4 when you cast your line.
- Will tell you are out of bait when you run out instead of next time you cast.
- When you run out of bait the vendors will re-stock.

	NOTE that if you already have a Fishing Pole and a Bait Bucket, the
	vendors will not restock those items, but they will restock bait if they
	were out. If you are out a bucket (you probably have a pole since you
	just ran out of bait) then they'll restock a bait bucket too.

You still have the same chance to catch fish (or cool items) as before (+10%)
but when you do catch fish, what you catch depends on what you have in your load
order:

(1) Morrowind Only or OAAB-DATA Only

	- 55% will be Crab Meat (you need food and this is the only basegame one)
	- 60% of the rest will be Small Slaughterfish (i.e. Fish Scales)
	- 40% of the rest will be Large Slaughterfish

(2) Tamriel-Data (with or without OAAB-DATA)

	- 15% will be Slaughterfish (60/40 Small/Large) and with OAAB some Fish Filets
	- 70% will be Common Fishes or Crab Meat (1/6 chance each)
	- 15% will be one of 3 Rare Fishes (33/33/33)

All fish you catch come with Fish Scales.

---------------
VERSION HISTORY
---------------

Version 2.0 ->

Well, when I made the first version, I made rare fishes the ones you'd have less
luck catching in a River (Cod for example since it's a sea fish) and since
Slaughterfishes are so common, I gave them a good chance to be caught. I had
completely forgotten that you can be affected by the first effect of an
ingredient when you eat it. This means that Slaughterfish meat is altogether bad
food, with its damage fatigue effect. So I re-did the chances for all the fish.
The rare fishes are now the ones that have 4 different effects, the "River" ones
are now called "Common" ones and they all provide positive-effects only.

I also increased the chance to catch something by 10% ->

	At zero fishing skill without bait, 2/10 chance to catch something
	At zero fishing skill with bait, 3/10 chance to catch something
	At max fishing skill without bait, 5/10 chance to catch something
	At max fishing skill with bait, 7/10 chance to catch something
	Bait is twice as effective from skill level 50 up (more or less same as base mod)

I also simplified the script a bunch, so there's always the possibility I have
introduced some bugs. And finally, I had to add a sound check to detect when you
swing your pole (Weapon Swish) otherwise when you got tired, and Ashfall started
reducing your maximum fatigue every second, you would get stuck catching fishes
non-stop. The sound check works pretty well, but it'll miss sometimes, just
swing again. This also fixes the mod triggering when you are not in fact
swigning your fishing pole.

Version 2.1 ->

It appears that for some Morrowind installations, the Weapon Swish sound is
either not playing at all, or play is delayed compared to when you swing your
weapon. In version 2.0 I added a sound-check each time you lost some fatigue
from swinging your fishing pole, but this was not working for at least one
person. In this new version, I made 2 ESP files. The base mod detects ONLY the
sound of you swinging your fishing pole to start fishing. This works fine for
me, but should this not work for you, there is an alternative ESP that uses
RacerPlume's method of fatigue detection. Note that if you are forced to use
fatigue detection, and are using Ashfall, you may end-up casting your fishing
pole non-stop until you move away from shore, should you become very tired as
per Ashfall (because Ashfall is lowering your fatigue every second).

------------
REQUIREMENTS
------------

You obviously need Fish With Fishing Poles (by RacerPlume) ->

	https://www.nexusmods.com/morrowind/mods/47230

Everything else is modular/optional ->

	To expose the Pole Fishing skill and to support OAAB/TRDATA ->

		You need MWSE with LUA installed, which comes with MGE-XE, see ->

			https://www.nexusmods.com/morrowind/mods/41102
			https://www.nexusmods.com/morrowind/mods/45468

		To see your Pole Fishing skill you also need Merlord's Skills Module:

			https://www.nexusmods.com/morrowind/mods/46034

	To get the Slaughterfish Filets you need the Expansion.esp, MWSE/LUA and OAAB-DATA ->

		https://www.nexusmods.com/morrowind/mods/49042

	To get extra fishes you need the Expansion.esp, MWSE/LUA and Tamriel-Data ->

		https://www.nexusmods.com/morrowind/mods/44537

------------
INSTALLATION
------------

This is now a BAIN installer.

Always install 00 Fish Expansion Core

And if fishing does not work, install ALSO 01 Fatigue Alternative Detection, which will replace the ESP with the Fatigue one.

Load the Expansion ESP AFTER the original mod if you want to catch more food.
Leave it disabled if all you need is to see your Pole Fishing skill.

------
THANKS
------

Ian (RacerPlume) for the base Fishing mod
OAAB/Tamriel-Data teams for the extra fish meats
Greatness7/Merlord/Necrolesian/NullCascase for help with LUA code
Merlord for the Skills module
Stripes for help with mwScript

-------
LICENSE
-------

Creative Commons Attribution 4.0
