
OpenMW Containers Animated v1.2.1

Based on MW Containers Animated by qqqbbb: https://www.nexusmods.com/morrowind/mods/42238
This mod adds open/close animation to all containers that should have animation.
Uses a native animated containers support feature from OpenMW 0.46, which allows to use ContainerOpen and ContainerClose animation groups to animate containers.
Implementation is very simple: just opening and closing animations with sounds, as in later TES games.

Notes:
1. OpenMW plays part of opening animation in the background, so you do not need to wait a half of second or more to open every container.
2. This mod does not provide any scripts and does not alter any container records, ESP file just registers sound records.
3. This mod can be used in any total conversion which uses Morrowind assets (such as Arktwend or Myar Aranath).
4. Obviously this mod is not compatible with original mod by qqqbbb.

Installation:
Just as any other mod according to this guide: https://openmw.readthedocs.io/en/latest/reference/modding/mod-install.html
Also "Optional" folder contains animated meshes for kollops.

History:
1.0:
Initial release.

1.0.1:
Fix drawer KF-file.

1.1:
Added RootCollisionNodes for all meshes excepts chests. May increase performance in exteriors a bit.
Fixed z-fighting for cupboard mesh.
Fixed missing animations for dwarven cabinet mesh.

1.2:
Replace closets, couldron and some chest meshes to smoothed versions.
Use simplified collisions for all animated containers, not just for sacks and barrels.
After migration from original Animated Containers mod, some containers could remain opened. Fixed.
Remove redundant stub Idle animation keys.
Fix some minor issues in closet meshes.

1.2.1:
Turn ESM file with sounds to the ESP file without dependencies, so OpenMW launcher can see it, fix file description.

1.2.2:
Fixed an initial state for xcontain_dwrv_desk00.nif.

Special thanks to CemKey for help with meshes!
