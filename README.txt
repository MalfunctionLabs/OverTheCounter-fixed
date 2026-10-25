OTCV 1.0.1 - Over The Counter, Vanilla port for Schedule I 0.4.7
==================================================================
Original mod: OverTheCounter (OTC) by hdlmrell
Port and new features: Malfunction Labs
No MeshVault needed: OTCV spawns its props itself (MeshVault's mesh format, built in).
License: CC BY-NC-SA 4.0 (see LICENSE.txt)


REQUIREMENTS
------------
- Schedule I 0.4.7
- MelonLoader 0.7.3 or newer
- S1API 3.2.1 or newer, including the S1APILoader plugin
- S1MAPI 2.0.1 or newer
- Optional: SteamNetworkLib 1.5.0 or newer, needed for multiplayer sync only

If something is missing, OTCV shows a popup on the main menu saying what to install and where.


INSTALL (manual)
----------------
Pick the file that matches your game branch:
  IL2CPP = the normal Steam version (most players)
  Mono   = the "alternate" beta branch

1. Install MelonLoader, then start the game once and close it.
2. Install S1API and S1MAPI (and SteamNetworkLib for multiplayer).
3. Copy the Mods folder from this zip into your Schedule I folder
   (the one that contains "Schedule I.exe"). Merge the folders if asked.
     Mods\OverTheCounter.Il2Cpp.dll   (or OverTheCounter.Mono.dll)
   MeshVault is no longer used. If you only installed it for OTCV, you can
   delete Plugins\MeshVault.Il2Cpp.dll (or .Mono.dll).
4. If you have the original OTC installed, this replaces it (same file name).
   Remove any other OverTheCounter.*.dll from Mods so only one copy loads.
5. OTCV already contains the OTC phone fix. If you have OTC046PhoneFix.dll in Mods,
   remove it.

Back up your saves before installing any mod:
  %USERPROFILE%\AppData\LocalLow\TVGS\Schedule I\Saves


MONO BUILD - PLEASE READ
------------------------
The Mono build compiles against 0.4.7 but has NOT been playtested.
These are IL2CPP-only and are NOT in the Mono build: the backpack, Trio products
and the Products app "B" badge.
Most likely to break on Mono: custom NPC setup (walk-ins, drifters, managers,
budtenders, Bella: names, mugshots, texting), manager inventories, and
returning items from a cancelled handover.
Please report Mono bugs (with your MelonLoader\Latest.log) on the Nexus page.


1.0.1
-----
- Fixed: the held item's name could sit on top of the HUD bars after going back
  to the menu and loading a save.


WHAT'S NEW IN OTCV (vs. OTC 2.0.10)
-----------------------------------
- Updated for Schedule I 0.4.7.
- Backpack: extra storage on the B key that catches pickups when your hotbar is full
  and can be searched by police. On by default (Mod Manager > Backpack; IL2CPP only).
- Counter: clicking a product on the counter hands it straight to the customer.
- Vic sends a daily laundering text with its own sound at 9:00 AM
  (VicDailyPrompt / VicDailyPromptTime / VicPromptSoundVolume in the config).
- "Trio" products: any product whose last three mixes are Viagor -> Cuke -> Mega Bean
  glows blood red, is worth 15% more, and gets red icons in every packaging (IL2CPP only).
- Products app: a small "B" badge marks products you are carrying in your backpack (IL2CPP only).
- Fixed: crash when opening Bella's handover screen.
- Fixed: a manager's clipboard panel staying open on other workers.
- Fixed (code review): rack, shelf and counter contents and placed-item links now survive
  save/load; register cash stays in its own counter; firing a manager no longer deletes
  what they carried; Static's Restore Service charges once; several co-op fixes (client
  checkouts, register balance, backpack saving, price edits, quest actions).

All original OTC features are kept: dispensaries (Westville Shack, Big Dispensary,
Supplier Warehouse), walk-in customers, budtenders, the GreenTab POS app, storefront
quests, managers and supply/distribution routes, Smart Fill, the Desperation system,
drifter encounters and more. See the original OTC page for the full feature guide.


CREDITS
-------
hdlmrell           OverTheCounter and MeshVault
ifBars             S1API (fork), S1MAPI, SteamNetworkLib
Malfunction Labs   0.4.7 port, OTCV additions

Bugs: report on the OTCV Nexus page, please, not to hdlmrell.
