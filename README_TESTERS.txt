RaidMem — Portable Windows Companion (Beta Test Build)
=======================================================

How to Run
----------
1. Double-click RaidMem.exe (Windows will ask for Administrator permission;
   this is required so RaidMem can read Raid.exe process memory).
2. If Windows Defender SmartScreen shows "Windows protected your PC"
   (normal for unsigned beta builds), click "More info" -> "Run anyway".
3. RaidMem will open in a dedicated desktop window using Microsoft Edge
   (or Google Chrome / your default browser if Edge is unavailable).
4. Launch Raid: Shadow Legends (either before or after opening RaidMem)
   and load into your Bastion. Click "Sync" in the top bar if your roster
   does not populate automatically within a few seconds.

Data, Cache & Logs
------------------
- Offline cache & logs are stored in:
  %LOCALAPPDATA%\RaidMem\raid_live_export.json
  %LOCALAPPDATA%\RaidMem\raidmem.log
- If you run into any issue, please share raidmem.log.

Game Updates (Optional Offset Override)
---------------------------------------
If a Raid: Shadow Legends patch changes memory offsets before a new
RaidMem.exe build is released, you can place an updated offsets.json
(or Il2CppDumper script.json) in the same folder as RaidMem.exe.
