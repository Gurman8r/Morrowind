  _________    ______ ____  ____ ______
 /_  __/   |  /     // __ \/_  _/ __/ /
  / / / /| | / / / // /_/ / / // _// /
 / / / ___ |/ / / //   ,_/_/ // /_/ /
/_/ /_/  |_/_|_/|_/_/|_| /___/___/____/


    ____  _________ __  _________ _______
   / __ \/ __/ __ // / / /_  _/ //_  ___/
  / /_/ / _//  __// / / / / // /  / /
 /   ,_/ /_/ __ // /_/ /_/ // /__/ /
/_/|_|/___/____//_____/____/____/_/

TAMRIEL REBUILT OFFICIAL README :: BUILD 22.11 - NOVEMBER 2022
====================================================
TABLE OF CONTENTS
====================================================

	I. INTRODUCTION

	II. INSTALLATION
		i.   Requirements
		ii.  Install Process
		iii. Registering Game BSAs
		iv.  Enabling Game Files
		v.   Updating Saved Games
		vi.  Recommended Mods

	III. PLAYING TAMRIEL REBUILT
		i.   Accessing the Landmass

	IV. KNOWN BUGS AND INCOMPATIBILITIES
		i.   Known Bugs
		ii.  Known Incompatibilities
		iii. Morrowind Rebirth, MGSO, and Replacer Conflicts

	V. TROUBLESHOOTING
		i.   Common Issues
		ii.  Known Bugs

	VI. NOVEMBER 2022 PROJECT STATUS

	VII. CREDITS & DISCLAIMER
		i.   Disclaimer & Copyright

====================================================
I. INTRODUCTION
====================================================

Thank you for downloading Tamriel Rebuilt!

Tamriel Rebuilt is a large fan project for The Elder Scrolls III: Morrowind. When Bethesda Softworks, the developers of the Elder Scrolls series, started designing the game towards the end of the 1990s, the original intent was to include all of the eponymous country's landmass in the game. As it turned out, this was too large a task and the scope was reduced to Morrowind's central volcanic island, Vvardenfell. Even so, the result was an enormous, colorful world that many, in our project and beyond, still consider one of their most memorable game experiences.

Our aim is to pick up where Bethesda left off: by creating the rest of its mainland, we are building Morrowind as it could have been, in a way that is truthful to the vision of the original developers. Rather than just providing a game world several times the size of the original, we want that world's vistas, stories, and people to be every inch as captivating as its example.

Tamriel Rebuilt is a long-term project. What took a team of paid, full-time developers several years obviously takes a group of volunteers longer. On the other hand we also have the luxury of not being bound by the same temporal and budgetary constraints that a game studio is subject to, which means we are free to undertake some things that would otherwise never become reality.

There is much to be created, much to be expanded and improved upon, and for that we need all the help we can get. If you love Morrowind and its world, if you are interested in the creation of mods or games, or if you just want a creative outlet in a lively online community, consider taking a look at how to join the project. (Join: https://www.tamriel-rebuilt.org/content/join)

We hope you enjoy our creation!

- The Tamriel Rebuilt Team

====================================================
II INSTALLATION
====================================================

----------------------------
i. Requirements
----------------------------
Before installing Tamriel Rebuilt, please ensure that you have the latest version of Morrowind (v 1.6820) installed, including both Tribunal and Bloodmoon, as well as the latest public release of Tamriel_Data (v 9.0 as of writing). No other plugins are required, but see the Recommended Mods section below.

Tamriel Rebuilt can be installed on either the vanilla (original) Morrowind engine or OpenMW, an open-source engine that seeks to reimplement and improve upon vanilla. It is highly recommended that vanilla users install Morrowind Code Patch as well, to ensure all quests work as intended.

Installation is almost the same for OpenMW, with an extra optional and semi-optional step, as indicated in the subsections.

Tamriel_Data: https://www.nexusmods.com/morrowind/mods/44537
Vanilla: https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition
OpenMW: https://openmw.org/en/
Morrowind Code Patch: https://www.nexusmods.com/morrowind/mods/19510

----------------------------
ii. Install Process
----------------------------
Tamriel Rebuilt comes packaged in the BAIN format, a folder structure designed to be automatically parsed by mod managers. Wrye Mash is a good option if you have experience with other managers. Beginners to Bethesda modding may have an easier time installing manually.

Vanilla / OpenMW (merged directory):
------------------------------------
To install TR, open the downloaded .7z file using 7-Zip, open the 00 Core directory, and move/extract its contents (including at least TR_Mainland.esm) to your Morrowind Data Files directory, which is under the same directory as Morrowind.exe. If prompted to merge folders, click Yes.

Note: The 00 Core directory also includes the files TR_Preview.esp, TR_Travels.esp, TR_Travels_(Preview_and_Mainland).esp, and TR_OldTravels.esp. These are DUMMY files, containing no content. They are only meant to overwrite old, deprecated plugins for players that are upgrading from older versions of Tamriel Rebuilt, and who may otherwise see errors from inadvertently leaving using the old plugins. You do not need to enable these plugins (see iv. Enabling Game Files section below).

OpenMW Only (separate directory):
---------------------------------
OpenMW provides support for mod directories outside of Data Files so that manual uninstallation is easy and clean. To follow this step, do the same as above but move/extract TR_Mainland.esm to a "Tamriel Rebuilt" folder in whichever directory you like. You should have Tamriel_Data in its own directory as well.

You need to register the folders of both Tamriel_Data and Tamriel Rebuilt inside openmw.cfg. Locate this file at:

	Linux: $HOME/.config/openmw
	MacOS: $HOME/Library/Preferences/openmw
	Windows: C:\Users\<USERNAME>\Documents\My Games\OpenMW

Search the file for the last line containing data=, and add the following lines below:

	data="<PATH>Tamriel_Data"
	data="<PATH>Tamriel Rebuilt"
	
...replacing <PATH> with the filepath where your Tamriel_Data and Tamriel Rebuilt folders are located. The double quotes are required. Save the file and exit.

(Alternatively, you might be interested in trying Mod Organizer 2, which works with OpenMW using this plugin: https://www.nexusmods.com/morrowind/mods/45642/) (Mod Organizer 2: https://www.nexusmods.com/skyrimspecialedition/mods/6194)

Optional Modules:
-----------------
Further optional modules can be found in "01 Faction Integration" and "02 Siege at Firemoth Compatibility Patch".

	- 01: TR_Factions.esp:  adds Telvanni Hortator and Ashlander Nerevarine quests to the mainland and modifies vanilla faction promotion requirements  
	- 02: TR_Firemoth_Vanilla_patch.esp:  needed when playing with the official mod Siege at Firemoth. Make sure to load after "Siege at Firemoth.esp" (see section "iv. Enabling Game Files" below)

----------------------------
iii. Registering Game BSAs
----------------------------

Vanilla:
--------
Unless already present*, you will need to make a one-time edit to the Morrowind.ini file in the game directory, instructing the game to load our game assets. To do this, open the INI file in any text editor, and navigate to the [Archives] section.

You should see a list of registered game archives from the Tribunal and Bloodmoon expansions. You must add these lines below the list of archives:

	Archive 2=TR_Data.bsa
	Archive 3=PC_Data.bsa
	Archive 4=Sky_Data.bsa

The number after Archive should be one higher than the previous entry. In most cases they will be 2, 3, and 4. Once that is complete, save and close the file. You only need to do this once.

(If you are using Mod Organizer 2, these lines won't register. Instead, see our applicable FAQ section here: https://www.tamriel-rebuilt.org/about/frequently-asked-questions/bsa) (Mod Organizer 2: https://www.nexusmods.com/skyrimspecialedition/mods/6194)

* Warning! Users of earlier versions of Tamriel_Data will also have to update their Morrowind.ini, since the names and number of BSAs changed in Tamriel_Data v9.0.

OpenMW:
-------
For OpenMW, you can follow the steps for vanilla then run the Morrowind Settings Importer in the Settings tab of the launcher. However, this may change some custom settings you have.

To add the appropriate settings manually, open openmw.cfg again and below the last line containing "fallback-archive=", add these lines:

	fallback-archive=TR_Data.bsa
	fallback-archive=PC_Data.bsa
	fallback-archive=Sky_Data.bsa

----------------------------
iv. Enabling Game Files
----------------------------
The final step before playing the new content is to enable the ESM and ESP files you selected. Open the launcher for Morrowind or OpenMW and ensure that Tamriel_Data.esm, TR_Mainland.esm, and your optional ESPs are ticked in the Data Files window/tab.

----------------------------
v. Updating Saved Games (for compatibility with a newer TR version):
----------------------------

Warning! We do not recommend updating older saves to TR version 22.11. Given that we significantly overhauled many parts of the mainland, there is a great chance that you will end up with a broken save. It is much safer to start a new character. However, if you wish to risk it, the instructions for updating old saves are below.

Vanilla:
--------
If you are updating Tamriel Rebuilt and intend to resume playing an existing saved game, you must first run the file patcher contained in the Tamriel_Data download and then undertake the additional steps outlined here (https://en.uesp.net/wiki/Morrowind_Mod:Morrowind_Modding_Wiki/Wrye_Mash#Using_an_Updated_Version_of_a_Mod) to resolve any potential errors. Please note, you will need to download and install the Wyre Mash utility to clean and repair your saved game using the method above as well as a Java Runtime Engine to use the file patcher.

OpenMW:
-------
OpenMW uses a different save format, so the file patcher is incompatible. However, the Wrye Mash part of updating is done automatically, so you can always load a saved game and hope for the best, fixing via console if necessary. We try to keep quest-related ID edits to a minimum. Without a compatible file patcher, though, OpenMW saves are unlikely to function well over the long run.

----------------------------
vi. Recommended Mods
----------------------------
We have a semi-regularly updated website page for recommended mods, found here (https://www.tamriel-rebuilt.org/recommended-mods). Patch for Purists and Morrowind Optimization Patch are essential mods to play TR without vanilla-based bugs.

Other notable mentions include the Tamriel Rebuilt Original Soundtrack by Rytelier and ASKII, which requires Morrowind Script Extender (MWSE), and all of the Landmass Mods, of which the two major ones are provinces developed by our sister project, Project Tamriel (https://www.project-tamriel.com/).

There is also the optional download for Tamriel Rebuilt called "TRMusic". These are older tracks than the official soundtrack, and they don't integrate as well with the other tracks. To install TRMusic, extract the music files into your Data Files/Music directory.

====================================================
III. PLAYING TAMRIEL REBUILT
====================================================

All Tamriel Rebuilt content will be accessible the moment you start a new game or load a saved game.

----------------------------
i. Accessing the Landmass
----------------------------
Most of our playable content can be found on the peninsular mainland east of Vvardenfell and a strip of land to the south of Vvardenfell. Newer content is focused in the south (Aanthirin, Roth Roryn, Armun Ashlands, and Velothi Mountains regions) and in the eastern cities of Firewatch and Helnim. 

You can cross the Inner Sea by boat from many ports through TR-added travel NPCs. These NPCs can generally be found close to the vanilla travel NPCs in the corresponding settlements:

    Anedhil (TR_m0_Anedhil) in Sadrith Mora
    Domiah (TR_m0_Domiah) in Ebonheart
    Gindrala Nethri (TR_m0_Gindrala Nethri) at Vivec Docks
    Ohmonir (TR_m0_Ohmonir) in Vivec Mages Guild
    Ysmund (TR_m0_Ysmund) in Dagon Fel

====================================================
IV. KNOWN BUGS AND INCOMPATIBILITIES
====================================================

----------------------------
i. Known Bugs
----------------------------
As Tamriel Rebuilt is a work-in-progress, be aware that there will be bugs and inconsistencies in our content, especially with much of it being made before our current standards. Here is a short list of the main bugs.

Global Map Cutoff and Crashes (Fixable):
----------------------------------------
Users playing on the vanilla game engine may notice that with Tamriel Rebuilt content installed, the global map cuts off abruptly at the edges. This is an in-game engine limitation, and both the Morrowind Code Patch and OpenMW address it. MCP has an option called Tamriel Rebuilt Map Fix, which extends the map and also fixes the frequent crashes that may occur when exploring distant regions. OpenMW natively supports an unrestricted map.

Landmass Abruptly Ends in the south and the West (Over Time):
-------------------------------------------------------------

Tamriel Rebuilt releases its lands expansion-by-expansion to slowly build out the entirety of the Morrowind mainland, while still allowing players to enjoy already finished areas. Since not all of Morrowind is released, our border areas will end abruptly in sea. If you wish to include unfinished areas in your game so as to give the map a nicer shape and to avoid looking at the sea voids, you will have to use in-development release files that are publicly available on our website. Ask us for advice, if you wish to do so.

Landscape and Other Inconsistencies (Over Time):
------------------------------------------------
Much of the released mainland was made many years ago, before planning standards were put in place. Thus, a lot of our older content may be stylistically inconsistent with content that was made more recently. We will address this in future updates.

Incomplete Questlines (In Progress/On Hold):
--------------------------------
We still plan to add some new questlines to Andothren, Firewatch, Armun Ashlands, and Necrom in coming bugfix releases.

The Telvanni and eastern Temple questlines were early creations and are incomplete. There are no plans to finish them until the rest of our landmass is completed.

Low FPS (In Progress):
----------------------
Some of our older areas or assets were created with little regard to optimization and, consequently, playability. As a result, areas such as Old Ebonheart, Roa Dyr, Akamora, and the Lan Orethan forest may suffer steep frame drops. While several changes have been made to models and areas, we plan to continue optimizing these areas and assets.

----------------------------
ii. Known Incompatibilities
----------------------------
Because Tamriel Rebuilt's landmass fills much of the empty space adjacent to Vvardenfell, it is naturally incompatible with any mods occupying the same space. Several other incompatibilities may result from mesh updates and overhaul changes such as those made by Morrowind Rebirth.

We have compiled a list of these conflicting mods for your reference. This list will continue to update as we become aware of changes to these mods and new incompatibilities within the mod community. If you find an instance of conflict, please report it on our bug tracker. (https://www.tamriel-rebuilt.org/bugtracker)

If you wish to play these mods alongside Tamriel Rebuilt, you will need to use a utility called TESFaith to move the landmasses manually. We unfortunately cannot offer support for this method, though there are other resources in the community that can help.

Landmasses that Conflict with TR_Mainland:
The Goblin Lab
N'Dib's Twilight
Inferno Island
Korobal Island
Island of Tusar
Hawkfir Island
Tree of Life
The Black Mill	
Morrowland
Booty Island
Moon's Spawn
Black Marsh
Darkshroud Keep
Journey's End
Snakebitten Island
Bloody Oath	
Roman City of Theopolis
Rafer: Sands of an Era
Lilligue Island
Helios Keep
Isengard
Love in the Time of Daedra
Legend of Chemua
Tel Scelestus

Landmasses that will conflict with TR_Mainland eventually:
Silgrad Tower
Wizard's Island
BYG
Annastia
Velidon
Dulsya Isle
Five Toes
Havish		
Great Shoals
Stagenau Isle
Western Island

----------------------------
iii. Morrowind Rebirth, MGSO, and Replacer Conflicts
----------------------------
Morrowind Rebirth is a popular overhaul for Vvardenfell and Solstheim, but it conflicts with Tamriel Rebuilt in several ways. Morrowind Rebirth overwrites some models and repositions them on Vvardenfell. This repositioning does not carry over to TR's landscape because we use the original models. Therefore, you may encounter objects with improper placement on the mainland. Morrowind Rebirth also rebalances many of Morrowind's items, spells, and foes, which can make TR's content overpowered in comparison. While it is possible to play Morrowind Rebirth together with Tamriel Rebuilt without game-breaking problems, neither we nor Morrowind Rebirth's author recommend it due to the reasons above.

The Morrowind Graphics and Sound Overhaul (MGSO) is outdated. It is not recommended by us or its author as it causes a wide variety of game and compatibility issues. There is still a tendency for people to download and play with it, however. If you choose to do so, any issues related to Tamriel Rebuilt should first be troubleshooted by removing MGSO.

Another conflicting mod is the Mountainous Red Mountain replacer, which causes major placement issues, especially around the Velothi Mountains. An alternative version of Mountainous Red Mountain can be found here (https://www.dropbox.com/s/6rakhzt9c0d7epx/MRM-Non%20Pointy.rar).

As development of TR has progressed, our use of custom assets over vanilla assets has increased. Popular texture replacers will not affect these non-vanilla assets, so beware of quality and style mixing when you choose them.


====================================================
V. TROUBLESHOOTING
====================================================

----------------------------
i. Common Issues
----------------------------
When setting up Tamriel Rebuilt, you may run into several problems. These are listed below.

Missing Resources: Users who fail to register the BSAs correctly will often find that loading Tamriel Rebuilt will result in a lot of "missing meshes/animation" error dialog messages popping up on load, some even fatal. Please double-check your Morrowind.ini file to ensure our two Data archives are registered properly; otherwise the game won't load.

Windows Permissions Errors: Users who play Morrowind on Windows operating systems may find that despite their efforts, the game will still churn out missing mesh errors. This is a result of the Windows User Account Controls. Either disable UAC through the Control Panel, or install the game in a directory other than "Program Files".

----------------------------
ii. Reporting Bugs
----------------------------
As Tamriel Rebuilt is a work-in-progress, it is inevitable that one will discover bugs along the way. These can range from small issues such as placement errors (floating, bleeding, and "caspering" objects), to more serious problems like broken quests, dialogue, and land tears. It is crucial to report these to us so that they may be fixed in subsequent updates.

It is recommended that you use the game's built-in beta comment feature to report bugs. You must first define the Beta Comment File in your Morrowind.ini by searching for:

	Beta Comment File=

...and typing in the name of the text file after the = sign. When you find a bug in the game, open the console using the tilde (~) key, click on the object in question, and type:

	bc "describe the bug"

...which will dump the output and object coordinates to the text file defined above. Repeat this procedure whenever you encounter a bug. You may then open the text file afterwards and copy its contents when you file a bug report on our bug tracker (https://www.tamriel-rebuilt.org/bugtracker).

====================================================
VI. NOVEMBER 2022 PROJECT STATUS
====================================================
As of November 2021, the latest build of Tamriel Rebuilt is version 22.11, a major release containing the expansions "Dominions of Dust", adding the city of Andothren and a vast badlands area to Vvardenfell's southwest; and "Embers of Empire", a complete overhaul of the cities of Firewatch, Helnim, and the surrounding hinterland. Combined, these expansions add or overhaul over 200 quests to TR.

Our next releases will mainly focus on bugfixing and the slow drive south to finish the Narsis District, the mainland holdings of House Hlaalu.

====================================================
VI. CREDITS & DISCLAIMER
====================================================

Making Morrowind's vision come to life is a colossal effort, undertaken by many fans over the course of Tamriel Rebuilt's twelve years in existence. We would like to thank all those developers, past and present for their contributions to this project.

Exterior Design
---------------
Acheron
Aeven
Andres Indoril
Animunculi
Arcandrith
Arthmodeus
Arvisrend
attackdrone
BarackOshizzle
battle_bison
blackbird
Cathartis
Chef
Cicero
CleverClothe
c0dacan0n
Codemonkey360
Cookiemonster16
DarkKnightComes
Denis418
Dexter
Draega07
EdBacon
EJRS
El Scumbago
Excuses and Accusations
FoxTamer
Fuzzy
Gez
G.M.K.
Gnomey
Haplo
Hemitheon
Hermit
Inferno_str1ke
joanasc
Juhazar
Katze
kebra
kingfish
Kothloth
Lady Nerevar
Jedak
Liliath
Moorkh
Mwgek
Juhazar
Jule
kapuhy
Kiteflyer61
Legolas55
Lord_Gallant
Lud
Melchior Dahrk
Meriyal
MinerMan60101
mojo187
Morden
Nairb
Nazz
Nemon
Nichevo
Noirgrim
Nomadic1
Peter_UK
Phenoix12
PoHa!
presh
president
Prometheus
Rats
Rockwell
Rodan
Scamp
selengor
Seneca37
Seran
Sevenup243
Sir Dave
SquallTM
Stalker
Swiftoak
Taniquetil
Teli
Thal
Theo
theviking
trifxn
Tyrion
Veet
Vegor
Vernon
Walt[FT]
wererat
Wolli
Zalzidrax


Interior Design
---------------
10Kaziem
6plus
Aaron
adamantum
Adanorcil
Adense
Aeven
agram
Aidan1470
Aleister
alex25
Am'Shak
Andres Indoril
AngryNord
Animuncul
Anneryl
Annon
Argoth
Ariss
Arthmodeus
arturs
Arvisrend
Ashstaar
Assassinace
Ataemus
attackdrone
Atrayonis
Avarr
Aveno
Ayedail
bas
battle bison
bDacc
Beef Puppy
Bero
bhhorton
Bill
blackbird
black0ut
Boznirith
Brannon the ilk
Bricktosser
Bugsby Bearkeley
C-A-G-E
CarbonCreations
carlthepimp
Cathartis
CdoubleOK
Chef
CherryGoat
Chin Music
christixn
Cicero
cire992
CleverClothe
c0dacan0n
Codemonkey360
Colhir
Corsair
daedren
DangerDog
Darkcorax
DarkEclipse
DarkKnightComes
Darth_Blade
Denis418
Dev Shah
Devil's Right Hand
DGSmds1
Dillonn241
Dinmenel
Divayth Fyr
doemaarwat
Dormichign64
Dragon
DrBongo
Dubba_D
EdBacon
Ede
EJRS
El Scumbago
ENIGMA*
Evil Eye
Excuses and Accusations
Exovian
franky702702'
Fremennik
Frun1987
G.M.K.
Garinator
garnath
Gez
Gnomey
GodizigelWinter
Graff
Grey
Griff93
gro-Dhal
Haplo
Harke the Apostle
Hayden
Hemaris
Hemitheon
Indoril
InfallibleDres
Infragris
Iskuss1418
Jackimoff Wackimoff
Jale
Jani
Jule
Kaiel
Katze
Khazar
Koma21
Kothloth
kretterzLac
Kynesifnar
Kyro
Lady Nerevar
laflamenca
Legoless
Leon
Leyawynn
Lord Elias
Lord_Gallant
LordGothren
Lucevar
Lud
Lumpag
lunareane
Magelord648
Magi
Magpie
Makiok
mariedanj
Mark
Massalinie
Matin Sanguine
matts05
Maurvir
meick
michaleson
MinerMan60101
Mirabell
mojo187
MoonAndStar
Mothergoose
Moyglass
Mr. Alligator
Mwgek
Myxinidae
Nairb
Nanu
NEENJA
Nemon
Neoptolemus
Nerano
Nerdevar
nick9999
Nichevo
Nirvayn
Nomadic1
Not
Odawacar
ohnoitsabear
Ola
Onoria
Osidian
Parker
PartiallySane
PaulShin
Peterboy
Peter
Petethegoat
Phenoix12
pianobadger
PoHa!
poiu
Praedator
presh
Prowler
Psypherious
Ragox
raandom
Rain In July
RandomPal
Rats
rayetaspen
RDV
Remiros
Resadyn
roerich
ropcm26
RyanS
Quentin Fortune
SACarrow
Saddboye
Sadi
saimol
Saint Olms
SamirA
Sand
Sandrew
Scamp
selengor
Seneca37
Serpentbyte
Serric
Shapeshiftr
Silvone Elestahr
sirrah
Sliced Bread
Sload
SlugZ
Snailsting
Sniper4
souldread
Stalker
starcrunch
Stripes
Stryker
Sultan of Rum
Swiftoak
Syzygy
talesofgames
Talias
Taniquetil
Teli
Terrifying Daedric Foe
Tes96
Thal
The Greatness
The guar man
the_cosmonaut
TheDarkKnight
The Laughing Gnome
Theo
theviking
Thrignar Fraxix
Tiefling
Timito
Tristior
Trotski
Tolkar
Tombomb47
Tyrant
Tyrion
uikaii
Uldar
UXO
Vegor
Veet
Vengyre
Vern
Vidi_Aquam
viKING
Waagenator
W-E-R-D-N-A
Why
WindEole
wishmaster
wojtek
Wolfrad
worsas
Wulf
Xui'al
Yeti
Yinnie
Zalzidrax


Quest Design
------------
10Kaziem
6plus
abby
AcrylicFrog
adamantum
Aeven
AliceL93
Am'Shak
Apoapse
Arkasas
Arvisrend
Atrayonis
Beave
BloodthirstyCrustacean
BomburPL
Boyos
Captain
Cicero
c0dacan0n
CogAndStar
ColaTheLionheart
crdgdr
DarkKnightComes
DestinedtoDie
Dev Shah
Dexter
Dillonn241
Dunmerius
El Scumbago
Envy123
Evil Eye
FlinSunset
Gesshoku
Gez
gro-Dhal
groza528
hammered on sujammer
Haplo
hardycore
immortal_pigs
Jackimoff Wackimoff
Jani
Jedak
jonado
Kaiel
Kevaar
Lud
MacBone
Mark
Marrinara_Sauce
Meej-Dar
Miamian
MMMowSkwoz
Mortimer
-MrWillis-
MSam
Nats482
NoMan
Not
Parker
PhDinSorcery
pianobadger
pkk
PoasterToaster
pralec
Rakanishu
randonaut
Rats
razenmaeher
Red Knight
Revane
Rot
Silvone Elestahr
slepana
Sload
starcrunch
steady_eddy
Steelgonads
Stryker
solarismin
Sultan of Rum
talesofgames
Taniquetil
Terrifying Daedric Foe
TheDarkKnight
Theo
Theron Udraer
theviking
The Violet Euphemism
Tristior
Tondollari
viol
Wanax
Why
Yeti
Zobator


Concept Art
---------------
10Kaziem
Aldegro
Ali
Almilexia
Ateiggaer
brianbusby
Burunduk
c0dacan0n
daedriclord
Dexter
Denise Bevz
DharmaPR
Dominic Zdenkovic
DONlimon
dyn0101
El Scumbago
Eldarion
Elfane
Emerald Skunk
Endoran
Euron
evergrey
Feivelyn
Floral Gemstar
Gez
Gihn
Gnober
Gnomey
GoblinMan
greendogo
Gustav
Harke the Apostle
Jadony
Jedak
Jelle
jonarus_drakus
Kaziem
Kieren
Lady Nerevar
lb003g0676
Lighter Than Some
LukeW
Lutemoth
Macar
MammaHyena
Melchior Dahrk
Morden
Morgoth
Mwgek
Myzel
Nalin
napoleoman
Nemon
Nirvayn
Nythrend
Obagovo
Pickles
PieXags
Revenant
SamirA
Shadowhawk
Steppenwolf
Swiftoak
Taijan
ThomasRuz
Túrelio
TyGl20
umbinc
VenuSprout
Wingate
Xeno
YanShun
Zadroter


Writing
-------
10Kaziem
6plus
Adanorcil
AlphaFemale
Andres Indoril
Apotheosis
Arslan
Arthmodeus
Arvisrend
Asylum
Atrayonis
BalinMinister
battle_bison
blackbird
Bloodthirsty Crustacean
Boompiee
C-A-G-E
Cicero
ColaTheLionheart
Craefish
Dazarlin
Deeza
Delemis
Dillonn241
Dunmerius
-Eidolon-
Earl
El Scumbago
Gez
Gnomey
Graff
gro-Dhal
grumble_dog12
Haplo
Harke the Apostle
Hemaris
Hemitheon
immortal_pigs
Ironed Maidens
Jacurutu
Jale
jkulhavy
Kevaar
klep
King-Morrowind
Lady Nerevar
Ludovic
Lutemoth
Macar
Merari
Miraclestone
Morgoth
Mortimer
Munkie
Nanu
Nomadic1
Not
nwo_viper
Ordie
Orix
Parker
presh
Psyborg
randonaut
Rats
redsrock
Rot
Sadi
Saibot
SirCabbage
Skootbot
slepana
Sload
starcrunch
storm_crow
Swiftoak
Taniquetil
Templar Tribe
Theminimanx
The_Skullpitter
The Violet Euphemism
The_Writing_Wraith
Theo
theviking
ThomasRuz
ThorFluff
Thunderforge
WellTemperedClavier
VarangainBard
vrover
Why
Xui'al


Asset Creation
--------------
10Kaziem
Adanorcil
Aeven
Aleister
Andres Indoril
AnrohaNexus
Arkhes
aro101
Asthaar
Asylum
Ateiggaer
avo1d
Barabus
c0dacan0n
Chef
Cicero
Dazarlin
detritus2004 (Khajiit faces)
Dongle
Dres
EP1CN3SS2
Eyeball88
FloorBelow
Garland
Geophysic2013
Gez
Gnomey
Haplo
Jelle
Kothloth
Kyneifnar
Lady Nerevar
Lestat DeLioncourt
Leyawynn
LondonRook
Lord Berandas
Maelan
Majra
Melchior Dahrk
Midgetalien
momoX
Morden
Mwgek
Myzel
Nalin
Negrodomeus
Neoptolemus
Nex
Petethegoat
Prometheus
Pug
Ragox
randonaut
Rats
RedFurryDemon
Remiros
revenorror
RuffinVangarr
R-Zero
Sandaron
Sandman
Shadow_Mimicry
Shishkinbar
Siberian Crab
Silaria (Argonian faces)
sirrah
Sissik-Wei
Slartibartfast
Stalker
Steppenwolf
Stripes
Superllama
Svartalfar
Swiftoak
T_nilc
Taniquetil
Varlothen
Veet
VenuSprout
Vernon
Vorrheis
Why
Wolli
worsas
Xeno
Zyndaar


Sound & Music
-------------
ASKII
daedriclord
Cicero
Don Bernardo
Dragonfly
Dummyplug
Eric Gordon Berg
Gesshoku
Leon
Macar
MAJ-12 MEDIA (MorrowindShorts)
Mannaz230
MorrowindShorts
Pug
Raincatcher
Rats
Rytelier


QA & Testing
------------
6plus
abot
AcrylicFrog
Adanorcil
Aeven
Aldurion
Aleister
Am'Shak
Amenophis
ArcticMetal
Arguss
Arvisrend
Ataemus
Bero
Bloodthirsty Crustacean
Boznirith
Bully
c0dacan0n
Cathartis
Chef
Cicero
Clovis the Lazy King
Cobalt
Corvus
crdgdr
damry
DarthGandalf
Delemis
Denis418
Dev Shah
Dillonn241
EdBacon
Eilmmom
Ember2528
esc
Evil Eye
Exovian
Factor
freefred1122
Fremennik
Frun1987
fstony
fufulames
Glisp
Gnomey
Haplo
Hemaris
Hidden Legend
immortal_pigs
Iskuss1418
Jackaljk 
JackDragent
Jackimoff Wackimoff
Jani
JennaK
jonado
Jule
JustComplains 
JohnnyMaverik
Kaann
Kaiel
Kalarak
Kayla123
Kevin
Khazar
Koma21
krazha
Kwama Conspirator
Lady Nerevar
Leon
Leyawynn
Lord Berandas
Malchik
mangoman
marius851000
Mark
Melchior Dahrk
Meriyal
Miamian
MinerMan60101
mojo187
Moonbeam
Mortalit
Mortimer
Mwgek
Myxinidae
Nalazdor Zaam
Napilon
Nemon
Nerano
nom
Not
nuclearwinter
OldFashionedGuy
Onmund803
opl2
Ormuni
Osidian
Osiris
Outlander3734
PartiallySane
paw-prints-in-the-mud
PeerOfKings
Peter
Petethegoat
Phenoix12
Pieniadz9
pralec
presto
Raddin
Ragox
Rakanishu
Randolph Carter
RandomTaffer
Rats
RedFurryDemon
Riuoku
Rod Uveges
Rot
Rung
RyanS
Saji
Sandaron
Scamp
Seneca37
SerpentByte
Sevenup243
Shadowhawk_the19th
Shask
sirrah
slepana
Sload
Snailsting
Sneab
SonOfKrampus
SpiderTheSpider
starcrunch
Stripes
Stryker
Sultan of Rum
Swiftoak
Taniquetil
Telumendur
Telvanni4Life
TennysonXII
Th1rt3en
Thal
The Maggot Guy
Thelliad
Theo
Theron Udraer
TheUndertaker
theviking
Thrignar Fraxix
tobyte
Tristior
ulmsllando
urm
Vern
Viltru
Vitruvian Guar
vivecs_tomb
W-E-R-D-N-A
Wanax
Why
Wyv
Wolli
xeth-ban
Yoae
Zadroter


Public Relations
----------------
Denis418
Kevaar
Lady Nerevar
Massalinie
MattTheBagel
Meriyal
-MrWillis-
Sultan of Rum
Swiftoak
the6thisstar


Web Hosting & Management
----------
Adanorcil
Ash
Atrayonis
ko2fan (Garfield)
Magamo
slepana
Zephyr


Asset Management
--------------
10Kaziem
Arvisrend
Atrayonis
Chef
Cicero
Haplo
Seneca37
Wolli


Special Thanks
--------------
Atrayonis (for reviving TR)
Ender (for founding TR)
Hrnchamd
The Imperial Library
Ken Rolston
Michael Kirkbride
Temple Zero

All of the early TR developers whose names are lost to history.

Bethesda for their awesome game.

... and of course all our fans and players!


----------------------------
i. Disclaimer & Copyright
----------------------------

Please credit the original authors first if the asset you want to use appears in this list (search using the corresponding Construction Set ID without suffix numbers); "edited" indicates that the meshes, textures, or text of the original asset have been altered or compressed in TR.

The following asset list aims to include:
	- By default, all separately released resources that were not directly contributed to TR by their authors but included based on their usage permissions, starting with the "Sacred East" release (June 2012).
	- Additionally, any assets from contributors past, present, or future who request separate documentation here.

This is retroactively documented before 2017 and therefore prone to oversights. Should anyone find they have been omitted from this list, please let us know.

Author:    Momo77
---------------------------------
Added Feb 2012, from: Momos Crane Resource - http://www.nexusmods.com/morrowind/mods/41074/?
IDs:    T_Com_SetHarbor_CraneLarge_01 to 03
    	T_Com_SetHarbor_CraneMiddle_01 to 02
    	T_Com_SetHarbor_CranePlatfL_01
    	T_Com_SetHarbor_CranePlatfS_01
    	T_Com_SetHarbor_CranePlatfVL_01
    	T_Com_SetHarbor_CraneSmall_01
Added Feb 2012, from: Momos Fishery Resource - http://www.nexusmods.com/morrowind/mods/41173/?
IDs:    T_Com_SetHarbor_DipNet_01 to 02
    	T_Com_SetHarbor_FishBeheaded_01 to 02
    	T_Com_SetHarbor_FishHanging_01 to 02
    	T_Com_SetHarbor_Fishnet_01 to 02
    	T_Com_SetHarbor_FishTrap_01
    	T_Com_SetHarbor_Rope_01

Author:    Slartibartfast
---------------------------------
Added Aug 2012, from: Smith Shed Resource - http://www.nexusmods.com/morrowind/mods/42183/?
IDs:    T_Imp_SetMw_X_SmithShed_01
    	T_Imp_SetNord_X_SmithShed_01
    	T_Nor_SetSkaal_SmithShed_01
Added Apr 2018, from: Imperial Plaza Resource - http://mw.modhistory.com/download-31-5968
IDs:    T_Imp_LegionCyr_X_Plaza_01 to 03 (edited)
    	T_Imp_LegionMw_X_Plaza_02 to 03 (edited)
    	T_Imp_LegionSky_X_Plaza_03 to 03 (edited)
Added May 2018, from: Well Diversified - http://mw.modhistory.com/download-7-15575
IDs:    T_Imp_LegionCyr_X_Well_03 to 04 (edited)
    	T_Imp_LegionMw_X_Well_03 to 04
    	T_Imp_LegionSky_X_Well_03 to 04 (edited)
    	T_Nor_SetSkaal_X_Well_01

Author:    t'nilc
---------------------------------
Added Aug 2013, from: Hookah - http://mw.modhistory.com/download-1-11970
IDs:    T_Rga_HookahApp_01
    	T_Rga_HookahFlavouredApp_01

Author:    Midgetalien
---------------------------------
Added Aug 2013, from: Stick Fences - http://www.nexusmods.com/morrowind/mods/42471/?
IDs:    T_Com_Set_FenceBriar_01 to 03
Added Dec 2013, from: Goblin Shaman - http://mw.modhistory.com/download-44-13318
IDs:    T_Mw_Cre_GobShm_01 (edited)

Author:    dongle
---------------------------------
Added Jul 2014, from: Elizabethan Galleon - http://mw.modhistory.com/download-44-2980
IDs:    T_Imp_SetHarbor_GalleonNavy_01 (edited)
    	T_Imp_SetHarbor_GalleonInLow_01 (edited)
    	T_Imp_SetHarbor_GalleonInUp_01 (edited)

Author:    Detritus2004
---------------------------------
Added Dec 2016, from: Khajiit Faces v2.0 - http://mw.modhistory.com/download-43-3301
IDs:    T_B_Kha_HeadMaleTR_02 to 09 (edited)
    	T_B_Kha_HeadFemTR_01 to 09 (edited)
    	T_B_Kha_HairMaleTR_01 to 02

Author:    Silaria
---------------------------------
Added Dec 2016, from: Sils Argonian Heads and Hair v1.1 - http://mw.modhistory.com/download-80-3324
IDs:    T_B_Arg_HeadMaleTR_02 to 07 (edited)
    	T_B_Arg_HeadFemTR_01 to 06 (edited)
    	T_B_Arg_HairMaleTR_01 to 07 (edited)
    	T_B_Arg_HairFemTR_01 to 04 (edited)

Author:    R-Zero
---------------------------------
Added Mar 2017, from: TR Silt Strider fix - http://www.nexusmods.com/morrowind/mods/43297/?
IDs:    T_Mw_Fau_Slstrid_01

Author:    Alaisiagae
---------------------------------
Added Jul 2017, from: Imperial Silver Armor Resource - http://mw.modhistory.com/download-56-6598
IDs:    T_Imp_Silver_Boots_01 (edited)
    	T_Imp_Silver_BracerL_01 (edited)
    	T_Imp_Silver_BracerR_01 (edited)
    	T_Imp_Silver_Greaves_01 (edited)
    	T_Imp_Silver_PauldronL_01 (edited)
    	T_Imp_Silver_PauldronR_01 (edited)

Author:    YarYulme
---------------------------------
Added Jan 2018, from: Nif Resources - https://www.nexusmods.com/morrowind/mods/43064/?
IDs:    T_Imp_Uni_SwiftcutSaber

Author:    Lochnarus
---------------------------------
Added Jan 2018, from: Elite Dark Brotherhood Helm v1.3 - http://mw.modhistory.com/download-80-7683
IDs:    T_De_UNI_PreyseekerHelm (edited)

Author:    Antares
---------------------------------
Added Jan 2018, from: Undead: Arise From Death - http://mw.modhistory.com/download-55-15310
IDs:    T_Mw_Und_Mum_02 (edited)
Added Dec 2019, from: Undead: Arise From Death - http://mw.modhistory.com/download-55-15310
IDs:    T_Glb_Und_SkelArise_01
    	T_Glb_Und_SkelArise_02
    	T_Glb_Und_SkelArise_03
    	T_Glb_Und_SkelArise_04
    	T_ScCrea_SkelRise_01 (edited)
    	T_ScCrea_SkelRise_02 (edited)
    	T_ScCrea_SkelRise_03 (edited)

Author:    Lougian
---------------------------------
added Jan 2018, from: Caverns Overhaul - https://www.nexusmods.com/morrowind/mods/42249/?
IDs:    T_Glb_Light_CaveRay01 to 12 (updated)

Author:    CemKey
---------------------------------
Added Dec 2018
IDs:    T_De_SetHla_X_Striderport_01

Author:    ch_devgroup
---------------------------------
Added Dec 2018
IDs:    T_De_RedBonemold_HelmOpen_01

Author:    Ao3
---------------------------------
Added Dec 2018
IDs:    T_De_SetHla_X_EntryFake_01
    	T_De_SetHla_X_Grate_01
    	T_De_SetHla_X_Waterspout_01

Author:    PikachunoTM
---------------------------------
Added Feb 2019
IDs:    T_Nor_UNI_Targe_Blooded
    	T_Com_UNI_KingOrgnumCoffer_01
    	T_Dae_UNI_Rueful_Axe
    	T_Dae_UNI_NebCrescen
Added May 2019
IDs:    T_Glb_Fauna_Photodragons_01

Author:    Nich/ZWolol
---------------------------------
Added May 2019, from: Correct UV Rocks - https://www.nexusmods.com/morrowind/mods/46104
IDs:    T_Mw_TerrRockRR_Rock_01 to 30 (edited)

Author:    Stuporstar
---------------------------------
Added May 2019, from Graphic Herbalism - MWSE and OpenMW Edition - https://www.nexusmods.com/morrowind/mods/46599
IDs:    T_Mw_Flora_HornLily_01 to 06
        T_Mw_Flora_Nirthfly03 to 05
        T_Mw_Flora_TimsaComeB01 to 04
        T_Mw_Flora_Meadowrye01 to 04

Author:    Tyddy
---------------------------------
Added Aug 2019, from: Bigger Temples - Urbanopticum of Vvardenfell - https://www.nexusmods.com/morrowind/mods/46184
IDs:    T_De_SetVeloth_Temple_03

Author:    Lurlock/Dragon32
---------------------------------
Added: Sep 2019
IDs:    T_Mw_CaveBone_Exit_00
    	T_Mw_CaveVM_TunnelBig_05
    	T_Mw_CaveVM_RoomBig_06
    	T_Mw_CaveVM_RoomBig_07
    	T_Mw_CaveVM_RockBridge_01
    	T_Mw_CaveVM_Doorway_00
    	T_Mw_CaveVM_Exit_00
    	T_Mw_CaveVM_Exit_01
    	T_Mw_CaveVM_RockForm_00 to 03
    	T_Mw_CaveVM_TunnelSml_05
    	T_Mw_CaveVM_RoomSml2_00
    	T_Mw_CaveVM_RoomSml3_00 to 02
    	T_Mw_CaveVM_RoomSml4_01 to 05
    	T_Mw_CaveVM_RockStal_00 to 05

Author:    Danke
---------------------------------
Added Dec 2019
IDs:    T_De_TelvCephalopod_PauldL_01 (edited)
    	T_De_TelvCephalopod_PauldR_01 (edited)
    	T_De_TelvCephalopod_GauntL_01 (edited)
    	T_De_TelvCephalopod_GauntR_01 (edited)
    	T_De_TelvCephalopod_Boots_01 (edited)
    	T_De_TelvCephalopod_Greaves_01 (edited)
    	T_De_TelvCephalopod_Cuirass_01 (edited)

Author:    Rubberman
---------------------------------
Added Dec 2019
IDs:    T_MW_DngBarrow_Stairs_01

Author:    Danea123
---------------------------------
Added Dec 2019, from The Demon of Knowledge - https://www.nexusmods.com/morrowind/mods/46126
IDs:    T_Dae_UNI_OghmaInfinium

Author:    IconsPNG
---------------------------------
Added Dec 2019, from iconspng.com - https://www.iconspng.com/image/83689/magic-circle-1
IDs:    T_Dae_UNI_OghmaInfinium (edited)
		
Author:    Remiros and Melchior Dahrk
---------------------------------
Added November 2020, from OOAB Data - https://www.nexusmods.com/morrowind/mods/49042
IDs:	tr_misc_ebony_cup.nif
		tr_misc_ebony_fork.nif
		tr_misc_ebony_knife.nif
		tr_misc_ebony_l_flask.nif
		tr_misc_ebony_platter.nif
		tr_misc_ebony_spoon.nif
		tr_misc_ebony_frosted.dds
		tr_misc_ebony_gold.dds
		tr_misc_de_g_bowl_01.nif
		tr_misc_de_g_bowl_02.nif
		tr_misc_de_g_pitcher.nif
		tr_misc_de_g_plate.nif
		tr_misc_de_g_platter.nif
		tr_misc_de_g_pot.nif
		tr_app_e_alembic.nif
		tr_app_e_calcinator.nif
		tr_app_e_mortarpestle.nif
		tr_app_e_retort.nif
		tr_w_dae_throwknife.nif
		tr_w_goblin_arrow.nif
		tr_w_huntsman_arrow.nif
		tr_w_ice_arrow.nif
		tr_w_orcish_arrow.nif
		tr_w_silver_halberd.nif

Author:    YarYulme
---------------------------------
Added April 2020, from Nif Resources - https://www.nexusmods.com/morrowind/mods/43064
IDs:	tr_a_DwrvScrp_helmet.nif
		tr_a_DwrvScrp_bracer_w.nif

Author:    Quorn
---------------------------------
Added April 2020, from Quorn Resource Integration - https://www.nexusmods.com/morrowind/mods/43269
IDs:	tr_a_DwrvScrp_chest_C.nif

Author:    Heinrich
---------------------------------
Added Feb 2020, from Weapon Sheathing - https://www.nexusmods.com/morrowind/mods/46069
IDs:    tr_w_iron_dagger_02_sh.nif
		tr_w_iron_bsword_03_sh.nif
		tr_w_iron_dagger_02.nif
		tr_w_iron_bswrd_02_sh.nif
	
Author:    Lord Berandas
---------------------------------
Added Feb 2020, from Weapon Sheathing - https://www.nexusmods.com/morrowind/mods/46069
IDs:    tr_w_adamant_wakazashi_sh.nif
		tr_w_adamant_tanto_sh.nif
		tr_w_adamant_katana_sh.nif
		tr_w_adamant_dkatana_sh.nif
		tr_w_adamant_saber_sh.nif
		tr_w_adamant_lsword_sh.nif
		tr_w_adamant_dagger_sh.nif
		tr_w_adamant_bsword_sh.nif
	
Author:    InspectorJ, boaay, karlis
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_impact_door_01.wav (edited)

Author:    dirtydowntowner, djcdelahaye, 150112, schots, rutgermuller
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_impact_gate_01 (edited)

Author:    gevaroy
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_impact_glass_01 (edited)

Author:    AlanCat, SoundFlakes
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_impact_rock_01 (edited)

Author:    ToaTom
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_impact_vase_01 (edited)

Author:    Bertsz, kwahmah_02, kevinkace, ErikH2000
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_impact_wood_01 (edited)

Author:    AryaNotStark
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_obj_brush_01 (edited)

Author:    nettimato, dylanperitz
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_obj_dice_01 (edited)

Author:    benjaminharveydesign, ryujin95
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_obj_hammer_01 (edited)

Author:    omnisis, kyles, qubodup, celadon, rutgermuller
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_obj_irongate_01 (edited)
		TR_obj_irongate_02 (edited)

Author:    snardin42, 7778, Piggimon
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_obj_shovel_01 (edited)

Author:    aurea, pauliep83, neilraouf, craigsmith, jergonda, lezaarth 
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_obj_woodgate_01 (edited)
		TR_obj_woodgate_02 (edited)

Author:    robinhood76, zatar, jagadamba, rutgermuller
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_obj_woodslide_01 (edited)

Author:    OGsoundFX
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_sfx_ghost_01 (edited)

Author:    cell31-sound-productions, SoundFlakes
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_sfx_ghost_02 (edited)

Author:    aderumoro, slugzilla
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_sfx_ghost_03 (edited)

Author:    zatar
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_sfx_landslide_01 (edited)

Author:    jackmichaelking
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_sfx_wave_01 (edited)

Author:    SoundFlakes
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_sfx_woosh_01 (edited)

Author:    fission9, bulbastre
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_loop_abyss_01 (edited)

Author:    proxima4
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_loop_mtpeak_01 (edited)

Author:    robinhood76, klankbeeld, onderwish
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_loop_oldones_01 (edited)

Author:    kyles
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_crowd_applaud_01 (edited)

Author:    YleArkisto, unchaz, robinhood76
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_crowd_boos_01 (edited)

Author:    YleArkisto, joedeshon, robinhood76
---------------------------------
Added Sep 2020, from freesound.org
IDs:    TR_crowd_cheer_01 (edited)

Author: Enderal Team and Beyond Skyrim Assets
---------------------------------
permission granted by Larrian
Added Dec 2020, from Enderal https://www.nexusmods.com/skyrim/mods/77868/
IDs: T_Glb_Flora_Mangrove_01 to 04

Author:    ashtaar
---------------------------------
Added Dec 2020, from https://www.nexusmods.com/morrowind/mods/44398
IDs:    T_Dae_DngRuin_StatueMephala_01

Author:    TeamCutiKagouti
---------------------------------
Added Jan 2021, from https://www.nexusmods.com/morrowind/mods/44650
IDs: T_Com_Iron_Rapier_01
	T_Com_Steel_Rapier_01
	T_Imp_Legion_Dagger_02
	T_Com_Iron_Dagger_03
	T_Com_Steel_Dagger_02

Author:    Zobator
---------------------------------
Added Feb 2021, from https://www.nexusmods.com/morrowind/mods/45489/
Key replacement models

Author:    Ruffin Vangarr
---------------------------------
Added May 2021, from https://www.nexusmods.com/morrowind/mods/49534
Daedric helmets

https://www.freesoundeffects.com
---------------------------------
Vermai Sound effects (stock sound Jaguar)

https://sketchfab.com/3d-models/spyglass-b27ebbf423ae431f9dac6ab2c8790515
---------------------------------
"Spyglass" (https://skfb.ly/onnWu) by Miguel Salgueiro is licensed under Creative Commons Attribution-NonCommercial (http://creativecommons.org/licenses/by-nc/4.0/).

Author:    Echo
---------------------------------
Added Aug 2021, from Imperial Library 20th Anniversary Contest - https://www.imperial-library.info/content/dravins-rules
IDs:    TR_m4_Bal_LairVaultBook (Dravin's Rules, edited)

Author: Miguel Salgueiro
---------------------------------
From: https://skfb.ly/onnWu, licensed under Creative Commons Attribution-NonCommercial (http://creativecommons.org/licenses/by-nc/4.0/)
IDs:   T_Com_Spyglass01 (edited)

Author:    Reizeron
---------------------------------
Added Sept 2021, from:     Brevur of Balmora - Finally Some Good Statue Mod https://www.nexusmods.com/morrowind/mods/47557
IDs:    T_De_SetHla_F_Plaque
	T_De_Set_StatueBevur
	
Author:    Spok
---------------------------------
Added June 2022, via OAAB_Data
IDs:	T_Imp_LegionMw_X_Window_01
	T_Imp_LegionMw_X_Window_02

Author:    Chainy
---------------------------------
Added via OAAB_Data
scorch mark decals

Author:    Kiteflyer61 and Archipel de Pertevue
---------------------------------
Added via OAAB_Data
archery targets

Author: RubberMan
---------------------------------
Added June 2022, via OAAB_data
IDs:	T_Imp_FurnM_WeaponRack_01-02


Tamriel Rebuilt is a not-for-profit development team made up entirely of fans. We are not in any way, shape, or form associated or affiliated with Bethesda Softworks™, Zenimax, or any other entity involved in Morrowind's original development. The Elder Scrolls is a registered trademark of Bethesda Softworks. All additional content produced outside Bethesda Softworks and the TES Construction Set remains the intellectual property of its creators.

All rights to original game assets belong to Bethesda Softworks. Additional assets created for Tamriel Rebuilt are the property of their creators first, and the organization second. The following resources should only be used in mods with a dependency on Tamriel_Data: Molecrab, Riverstrider, Telvanni Cephalopod. All other assets are free to use and redistribute in other modifications provided that their original author (where applicable) or Tamriel Rebuilt are duly credited.
The content of this archive is © Tamriel Rebuilt Community 2001-2021.
http://www.tamriel-rebuilt.org


Rev. 22.11
Updated 21 Nov. 2022
