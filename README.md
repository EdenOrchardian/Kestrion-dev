# Kestrion: Beta channel

**Early builds of Kestrion, the real-time strategy game where you design every ship you command.**

This repository is where **Beta** releases are published: new features, balance changes and fixes, before they reach everyone. Betas are tested builds, but they are rougher than Stable ones. Expect the odd bug, and please tell us about it.

Looking for the regular game? The **Stable** releases are at **[Kestrion-release](https://github.com/EdenOrchardian/Kestrion-release)**.

## Joining the Beta

1. Install Kestrion: from the [Stable releases](https://github.com/EdenOrchardian/Kestrion-release/releases/latest), or from the [newest Beta here](https://github.com/EdenOrchardian/Kestrion-dev/releases/latest).
2. Get the **Beta code** from our Discord.
3. In the game, open **Settings > Updates**, type the code, and switch the channel to **Beta**.

From then on the game offers you every new Beta. It always asks before downloading anything.

**Leaving the Beta:** switch the channel back to **Stable**. You stay on your current version until Stable catches up; nothing is downgraded behind your back. To go back right away, use **Settings > Updates > Go back to the previous version**.

## Download

Under **Assets** of the [latest Beta](https://github.com/EdenOrchardian/Kestrion-dev/releases/latest):

- **`Kestrion-<version>-setup.exe`**: the installer.
  - **Express** installs into your own user folder.
  - **Custom** lets you choose the folder and the shortcuts.
  - No administrator rights needed.
- **`Kestrion-<version>-win-x64.zip`**: the portable version.

**Windows will say "Windows protected your PC".** The installer is not signed with a paid Windows certificate yet. Click **More info**, then **Run anyway**, after checking the file if you like (below).

**Requirements:** Windows 10 or 11 (64-bit).

## How a Beta becomes Stable

When a Beta has proven itself, the **exact same files** are promoted to Stable, byte for byte, with no rebuild. What Beta testers played is exactly what everyone else gets. Your testing really does decide what ships.

## What we are building

Kestrion is made by **EdenOrchardian**:

- A strategy game about **designs and decisions**, not grinding or paying.
- An **AI that never cheats**: it only sees and does what a player could.
- **Fair multiplayer** where every player runs the exact same simulation.
- **Privacy and safety first**: no trackers, no data collection, **Hide my IP**, signed updates, and a security review for everything that touches the internet.

## Made with AI, used properly

I always wanted to build a game, but never had the time or the expertise to do it alone. Kestrion is made with **Claude**, Anthropic's AI, as a working partner.

AI tools have been misused plenty: low-effort copies, standing in for artists, things nobody checked. I want to use them the right way:

- the vision and every decision stay mine;
- the art is drawn by code from mockups I choose, not generated images;
- everything is tested and security-reviewed before it ships;
- and I'm open about it.

The aim: something interesting and unique that could not have existed otherwise. The full story is in the [Stable README](https://github.com/EdenOrchardian/Kestrion-release).

## Checking your download

Every file is listed in **`SHA256SUMS.txt`** and signed with our release key (minisign format), the same key as the Stable releases.

**Our public key** (key id `6B4826021ADD7830`):

```
RWQweN0aAiZIa/zdL8dDf65GIuVV6kkLvVnUnoUITMVKKxAEHaMgN+t8
```

```
Get-FileHash .\Kestrion-<version>-setup.exe -Algorithm SHA256
minisign -Vm Kestrion-<version>-setup.exe -P RWQweN0aAiZIa/zdL8dDf65GIuVV6kkLvVnUnoUITMVKKxAEHaMgN+t8
```

**If the key you see anywhere ever differs from this one, do not run the file, and tell us.**

## Reporting bugs

Beta testers are the reason Betas exist. On our Discord, tell us:

- what you did and what happened;
- your version (shown in **Settings**);
- for a multiplayer match that fell out of sync, the `.kdesync` report the game saves.

"This felt great" is useful feedback too.

---

*This repository only holds releases. The game's source code is not public.*
