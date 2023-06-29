Multiple Teleport Marking Mod for OpenMW & Tamriel Rebuilt
Tamriel Rebuilt 2101 update


Contents:

  "MultiMarkOMW-1.3-TR2101.esp"
	-- v1.3 updated for TR 21.01
	   use this instead of the non-TR version, not both


2101 Changelog
- updated 4 new cells and 4 changed cell names
- fixed bug affecting newest interior cells R-Z

1912 Changelog
- added support for the new TR release

1807 Changelog
- added support for the new Old Ebonheart region
- now forbids teleportation when Tamriel_Data does

1709 Changelog
- updated cell names for 1709
- now forbids teleportation when TR does



-------------------------------------------------------------------

Full readme:

This is Marcel Hesselbarth's classic Multiple Teleport Marking Mod 
(http://mw.modhistory.com/download--3898) modified in order to work 
in OpenMW (0.41), though it will also work in the original engine. 
It replaces the vanilla Mark and Recall spells and adds 11 more slots 
to mark and recall to any location in the original game (and also 
in TR with the corresponding version). The original Mark/Recall slot
still works for unknown locations added by other mods.

Requires Tribunal and Bloodmoon.


Limitations:
There are a couple more limitations to work around bugs in current OpenMW:
  - only works with the original game's Mark/Recall spells and objects,
  - the two unused summon spells are taken up for the new Mark/Recall effects, 
    this will conflict with any mod that uses them to add custom summon spells.
  Besides these, most of the original mod's limitations still apply:
  - only one Mark can be set in places added by other unpatched mods,
  - the marks are not shown on the map,
  - the viewing angle cannot be restored.


Usage and credits:
  Refer to v2.2 -- all credits go to Marcel Hesselbarth for making the mod.
  This is just a tweak. The additional support for TR areas was also made 
  using his perl script found in "Teleport_Generate_Scriptcode". If you want 
  to make a compatibility plugin for another mod, see "Teleport_plugin_skelet" 
  for his example.


Changelog:
v1.3 - fixed script _getPosition from v1.2
v1.2 - scripts _getPosition and _infoPosition have been made slower to accommodate
       bigger add-ons (Skyrim and Stirk cells need more time). This slows down the 
       recall menu display and makes it stutter briefly, so if you don't use these 
       province mods you can stick to v1.
v1   - 