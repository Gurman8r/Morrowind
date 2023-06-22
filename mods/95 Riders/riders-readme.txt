Riders						0.62
----------------------------------------------------------

Adds guar rider NPCs to exteriors.


----------------------------------------------------------
	REQUIREMENT
----------------------------------------------------------
Vanilla: requires MCP feature "Improved animation support" 
	 in "Mod specific" category. NOT enabled by default!
	 if you didn't specifically pick that option it's 
	 not installed and you need to reapply the code patch.

openMW:  natively supports the feature after v0.46.
	 expect animation issues depending on version
----------------------------------------------------------

Current version adds a few patrols near Vivec or Ald Ruhn, 
some ashlander riders and the odd merchant.

Not a player riding mod! If you want a ride try Abot's Guars.


----------------------------------------------------------
	CONFLICTS
----------------------------------------------------------
The required MCP feature "Improved animation support" may 
conflict with some animation mods like Animation Compilation.
The only edit to exteriors is the addition of NPCs.
NPCs may not be able to find their way in heavily edited
landscapes, if one is stuck and annoys you just rest.


----------------------------------------------------------
	MODDING
----------------------------------------------------------
Guar set up as the Tail slot, so it doesn't have to hide a body 
part for humanoids, but equipment assigned with Tail parts isn't
supported by the CS and will become empty if you edit the plugin.
If you want to reuse the files for Tail consider working with a 
different bodyslot in the CS then editing the finished file.
There are animations for spears, bows and unarmed (guar bites).


----------------------------------------------------------	
	CREDITS
----------------------------------------------------------
rider anim by Lidicus in Guar Variants http://mw.modhistory.com/download-7-6222
saddle by Acid Basick from the same mod (originally Pegas Horse Ranch mod)

all other guars by EJ-12 from The Symphony https://www.nexusmods.com/morrowind/mods/43790


----------------------------------------------------------	
	Changelog
----------------------------------------------------------
0.62
- Ashlander4 no longer wears a shirt instead of his guar
- cleaned junk cell. note to self the tes3cmd delete of
  the shirt also removed activator flags (? unused now)
- xmountedGuar1.nif BB size was fixed whatever that meant
0.61
- possible fix for Caldera crash (removed AiActivate,
  but Caldera route will often get stuck until resting)
- openMW: disabled Hello when run in openMW engine
- openMW: added WalkBack keys now used by pathing
0.6
- anims: fixed twisted pelvis, idle leg jitter/bleeding
- mounts no longer turn to face the player during Hello, 
  sacrificed Turn animation keys (hardly used in vanilla)
- moved travel routes from NPC schedules into scripts, so
  they get stuck less in cells that don't have pathgrids
- 2 new hostiles, 2 more appear after defeating ashlanders
- repaired models that had broken normals or shading
- guar shadow shapes for the vanilla engine added
