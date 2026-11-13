> [!WARNING]
> **Beta Pre-Release:** This is an early portable Windows test build of **RaidMem**. Please report any bugs, crashes, or UI issues along with your `%LOCALAPPDATA%\RaidMem\raidmem.log`.

A standalone, zero-install Windows companion and gear optimizer for *Raid: Shadow Legends* (`Raid.exe`), powered by an out-of-process Il2Cpp memory reader. No Python or Node.js installation required.

---

### Download & Verification

Download **`RaidMem-Portable-Win64.zip`** from the Assets section below (`26.35 MB`), extract it, and run **`RaidMem.exe`**.

| Asset | SHA-256 |
| :--- | :--- |
| `RaidMem-Portable-Win64.zip` | `ED4CB8EA78E9BD24C117B5124B0FE4D4845294F23E564C1C946F943E4DB6094E` |

<details>
<summary>Verify checksum in PowerShell</summary>

```powershell
Get-FileHash .\RaidMem-Portable-Win64.zip -Algorithm SHA256
```

</details>

---

### Quick Start for Testers

1. **Extract** `RaidMem-Portable-Win64.zip` to any folder and double-click **`RaidMem.exe`**.
2. **SmartScreen (Unsigned Beta):** If Windows Defender SmartScreen shows *"Windows protected your PC"*, click **More info** → **Run anyway**.
3. **Administrator Prompt (UAC):** Click **Yes** when prompted — Administrator privileges are required to read `Raid.exe` process memory.
4. **Desktop Window:** RaidMem opens automatically in a standalone desktop window (via Microsoft Edge, or Chrome/default browser).
5. **Load Your Account:** Launch *Raid: Shadow Legends* (before or after opening RaidMem) and load into your Bastion. Your account should sync automatically; if not, click **Sync** in the top bar.

### Requirements
- **OS:** Windows 10 / 11 (64-bit)
- **Browser:** Microsoft Edge (preinstalled on Windows) or Google Chrome
- **Game:** *Raid: Shadow Legends* (`Raid.exe`)

---

### Highlights in `v0.1.0-beta`
- **Single-File Portable `.exe`:** Runs cleanly from any folder with no external runtime dependencies.
- **Live Memory Sync & Multi-Account Support:** Reads champions, artifacts, accessories, account resources, Great Hall/Arena bonuses, and live game state directly from `Raid.exe`.
- **Gear Optimizer & Exports:** Build solver (`effective_damage`, `effective_hp`, `speed`, `balanced`) and full CSV/JSON/ZIP account export.
- **Drop-In Game Patch Override:** If a *Raid* game update shifts memory offsets before a new release is posted, place an updated `offsets.json` (or Il2CppDumper `script.json`) in the same folder as `RaidMem.exe`.

---

### Logs, Cache & Reporting Issues
- Local cache and logs are stored per-user at:
  - `%LOCALAPPDATA%\RaidMem\raidmem.log`
  - `%LOCALAPPDATA%\RaidMem\raid_live_export.json`
- If something breaks or fails to sync, please include your `raidmem.log` and whether `Raid.exe` was already in the Bastion when reporting!
