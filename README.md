# Prison V2P (Panopticon) - project files

Version 1.0.16 | Made by MrLovac

**Download:** green **Code** button > **Download ZIP**.

## What this is

The Unreal Engine 5.5 level of the Prison V2P map for Bodycam, with its own meshes, as an example you can open,
study, change and rebuild into your own map. Only the files the level uses are here (the level + 75 meshes).

## What you need

- Unreal Engine 5.5
- The Bodycam Map Kit (an Unreal project with stand-ins for the game's own materials, the hardpoint zone and the
  build script). This level places the game's own assets by their game paths; they are NOT in this download, the
  Map Kit has stand-ins for them and the game supplies the real ones when you play.
  The Map Kit download is being cleaned for public release and will be linked here.

## How to open it

1. Close Unreal.
2. Copy the `Content` folder of this download into the Map Kit folder (next to `BodycamSandbox.uproject`), allow merge.
3. Open `BodycamSandbox.uproject`, then `Content/Sandbox/PrisonV2P/PrisonV2P_BP`.

## How to build it into a map

Save your changes under a NEW name (File > Save Current Level As, `Content/Sandbox/<Name>/<Name>_BP`), close
Unreal, and in Git Bash in the Map Kit folder:

    bash Scripts/newmap.sh <Name> "<Name players see>" <screenshot.png> 0.1.0

Please do not re-upload it as "Prison V2P"; make it your own.

## What is in the level

- Hardpoint: 1 HardPointZone + its BP_PointZonePreview actors (`Content/GM/Gamemode/HardPoint`).
- Team spawns: PlayerStart actors tagged 1 or 2.
- Walls/floors use the game's Concrete physical material, bars Metal (bullets stop); remove the overrides for the
  PAPERBACK behaviour (bullets go through).

## Links

- The map: [nexusmods.com/bodycam/mods/56](https://www.nexusmods.com/bodycam/mods/56)
- Map importer: [lovac.github.io/bodycam-map-importer](https://lovac.github.io/bodycam-map-importer/)

## Credits

- MrLovac - the Prison V2P level, its layout and the meshes in this download (free to study and change for your own
  Bodycam maps; please credit "Prison V2P by MrLovac" and do not re-upload it unchanged).
- Reissad Studio - Bodycam. The level references the game's own assets by path; none of them are included.
- Epic Games - Unreal Engine 5.5. Tools written with AI assistance (Claude, by Anthropic).

Fan-made, not made, supported or endorsed by Reissad Studio.
