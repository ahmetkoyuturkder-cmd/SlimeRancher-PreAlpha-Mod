<img width="1920" height="1080" alt="SlimeRancher-2026-05-26-10-21-19-17" src="https://github.com/user-attachments/assets/939d1047-b2d5-45f5-9c44-da1fb1265fb4" />
<img width="1920" height="1080" alt="SlimeRancher-2026-05-26-10-20-48-40" src="https://github.com/user-attachments/assets/650cc38c-20da-4257-b91c-8e7ec2a435a3" />
<img width="1920" height="1080" alt="SlimeRancher-2026-05-26-10-21-34-87" src="https://github.com/user-attachments/assets/46b8d087-6320-4085-a044-85b8b90af35c" />
<img width="1920" height="1080" alt="SlimeRancher-2026-05-26-07-55-46-68" src="https://github.com/user-attachments/assets/26aaeda4-863f-49c0-be7b-b95af5750f62" />
<img width="1920" height="1080" alt="SlimeRancher-2026-05-26-10-21-56-91" src="https://github.com/user-attachments/assets/be303e55-f2d8-4010-926a-eaca90508a87" />
# Slime Rancher Pre-Alpha Mod v0.0.1
**by Furkaiko**

> The world's first mod for Slime Rancher Pre-Alpha v0.2.1 (December 2015).

---

## ⚠️ Requirements
This mod only works with **Slime Rancher Pre-Alpha v0.2.1**.
You can find the pre-alpha build here: [Slime Rancher Pre Alpha on itch.io](https://granvizier.itch.io/slimerancherprealpha)

> Note: This build is not officially distributed by Monomi Park. Use at your own discretion.

---

## What is this?

Slime Rancher Pre-Alpha v0.2.1 was an early build of the game released in December 2015, before the game entered Early Access on Steam in January 2016. This build has been largely forgotten and undocumented — and until now, no one had ever modded it.

This mod was created by reverse engineering the game's `Assembly-CSharp.dll` using dnSpy, and injecting a custom DLL at runtime. No BepInEx was used (it doesn't work on Unity 5.2). Everything was built from scratch.

---

## Features

### 🎮 Cheat Menu (F4)
- **Noclip / Free Fly** — fly anywhere in the map
- **Money +10000** — add money instantly
- **Fill Energy / Health** — max out your stats
- **Clear Radiation** — remove all radiation
- **Keys +5** — add slime keys
- **All Upgrades + Jetpack** — unlock everything
- **Unlock All** — unlock all areas (Grotto, Overgrowth, etc.)
- **Daytime / Nighttime** — change time of day
- **Speed control** — 1x to 5x game speed
- **Pause / Resume**
- **Coordinates display** — see your X Y Z position

### 🐌 Slime Spawner
Spawn any slime directly — including ones not found in this area:
- All base slimes (Pink, Rock, Tabby, Boom, Rad, Phosphor, Hunter, Honey, Puddle)
- Gold Slime, Tarr
- All Largo combinations

### 🍎 Food to Inventory
Add any food item directly to your vacpack inventory:
- All vegetables and fruits
- Chickens (Hen, Rooster, Elder, Stony, Briar)
- Prickle Pear — exists in the files since v0.2.1, long before its official release!

### 📦 Special Items
Spawn special objects:
- Keys, Crates (Reef, Quarry, Moss, Desert)
- Exchange Crates
- All Plorts
- Water, Scarecrow

### 🐊 Gordo Spawner
Spawn any Gordo in the game
### 🌍 Multi-Language Support
- English
- Turkish (Türkçe)
- Spanish (Español)

---

## Controls

| Key | Action |
|-----|--------|
| F4 | Open/Close menu |
| F5 | Toggle Noclip |
| F6 | Refresh/Rescan |
| Space | Fly up (noclip) |
| Left Ctrl | Fly down (noclip) |
| Left Shift | Speed boost (noclip) |

---

## Installation

### Steps
1. Download the `Pre-Alpha Mod v0.0.1.zip` from [Releases](../../releases)
2. Extract the zip
3. Go to your Slime Rancher Pre-Alpha folder
4. Place `Noclip.dll` here:
```
SlimeRancher_Data\Managed\Noclip.dll
```
5. **Back up** your original `Assembly-CSharp.dll` first!
6. Replace `Assembly-CSharp.dll` with the one provided:
```
SlimeRancher_Data\Managed\Assembly-CSharp.dll
```
7. Launch the game — it may take up to 30 seconds to load and may appear unresponsive, this is normal. Wait for it to fully load.
8. Press **F4** to open the mod menu!

### To Uninstall
Replace `Assembly-CSharp.dll` with your backup and delete `Noclip.dll`.

---

## Interesting Findings

While making this mod, several interesting things were discovered about this early build:

- **Hunter Slime** exists in the game files but has no unique model yet — it uses the Tabby Slime model. The camouflage mechanic is not implemented. Slimepedia entry shows "TBD" for Slimeology, Rancher Risks, and Plortonomics.
- **Prickle Pear** exists in the game files since v0.2.1, long before its official release in a later update. It was originally planned as Rock Slime's favorite food.
- **The Pit** expansion area exists in the code but was removed before this version. It was located east of the Grotto and had only 2 plots.
- **Rad Slime** is fully present and functional despite Indigo Quarry being removed in v0.2.0.
- **Honey Slime** and **Hunter Slime** are fully coded but rarely spawn naturally in this build.

---

## Technical Details

- **Game version:** Slime Rancher Pre-Alpha v0.2.1 (December 18, 2015)
- **Unity version:** 5.2.2f1
- **Mod type:** DLL injection via modified Assembly-CSharp.dll
- **Tools used:** dnSpy, Visual Studio C# compiler (csc)
- **BepInEx:** Not used (incompatible with Unity 5.2.2)

---

## Reddit Post
[Hunter Slime Prototype Found in Slime Rancher Pre-Alpha v0.2.1](https://www.reddit.com/r/slimerancher/comments/1toddbv/hunter_slime_prototype_found_in_slime_rancher/)

---

## Disclaimer
This mod is for the Pre-Alpha build of Slime Rancher, not the official release. Slime Rancher is developed by Monomi Park. This project is not affiliated with or endorsed by Monomi Park.
