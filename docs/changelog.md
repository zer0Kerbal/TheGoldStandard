---
permalink: /Changelog.html
title: The Change Log
description: The Opening Credits, and the closing credits, plus the first of two (or is three) end credit scenes
tags: changes,changelog,change-log,page,kerbal,ksp,zer0Kerbal,zedK
---
<!-- hdr-changelog.md v1.0.0.1
The Gold Standard (GOLD)
created: 13 May 2022
updated: 05 Nov 2022
CC BY-ND 4.0 by zer0Kerbal -->  
﻿# Changelog  
  
| modName    | The Gold Standard! (GOLD) by Dewar                                |
| ---------- | ----------------------------------------------------------------- |
| license    | CC-BY-NC-SA-4.0+ARR                                               |
| author     | Dewar and zer0Kerbal                                              |
| forum      | (https://forum.kerbalspaceprogram.com/index.php?/topic/203990-*/) |
| github     | (https://github.com/zer0Kerbal/TheGoldStandard)                   |
| curseforge | (https://www.curseforge.com/kerbal/ksp-mods/TheGoldStandard)      |
| spacedock  | (https://spacedock.info/mod/963)                                  |
| ckan       | TheGoldStandard                                                   |

* 📌 Pinned
  * Dependencies (to add functionality to stock parts):
    * [ModularManagement (MM)](https://www.curseforge.com/kerbal/ksp-mods/ModularManagement) or [Module Manager](https://forum.kerbalspaceprogram.com/index.php?/topic/50533-*/)
  * can now search for `gold` or `tgs` in editors to find parts

## Version 1.6.4.0-release - `<Thank you Dewar>`

* Released
  * 08 Jun 2023
  * for Kerbal Space Program 1.12.5
  * by [zer0Kerbal](https://github.com/zer0Kerbal)

### Change Summary 1.6.4.0

* fixed small tanks abandonment issues with _much_ couch time
* The Gold Smelter's Cooling Conundrum should now be resolved, it needed extra heavy duty cooling fluid and much larger cooling lines!
  * thank you to forum user: Bizobinator for reporting the issue
* can now search for `gold` or `tgs` in editors to find parts
* Add localization: Mexican Spanish (Español Mexicano) [JamesErvin-5](https://github.com/JamesErvin-5)
* upscale flags and convert to .dds
  * add golden version
* cleaned up tags
* clean, lint, modernize
* update documentation
* update stock config patch to remove redundant patch

### Changes 1.6.4.0

#### Parts 1.6.4.0

* The Gold Smelter's Cooling Conundrum
  * should now be resolved
  * extra heavy duty cooling fluid was added
  * much larger cooling lines were required!
  * thank you to forum user: Bizobinator
  * [GoldSmelter.cfg] 1.6.4.0
* cleaned up tags
* clean, lint, modernize
* closes #73 - [BUG] Gold Smelter Cooling Conundrum

#### Config 1.6.4.0

* add headers
* fixed small tanks abandonment issues with _much_ couch time
  * update stock config patch to remove redundant patch
* closes #70 - PartLoader WARNING: surface attach node is defined more than once!

#### Flags 1.6.4.0

* Update
  * upscale
  * convert to .dds
    * [TGS-Black.dds]
    * [TGS-White.dds]
* Add
  * [TGS-Gold.dds] -  golden version

#### Localization 1.6.4.0

* Add
  * Mexican (Mexicano)
    * [es-mx.cfg] v1.0.0.0
    * Gracias [JamesErvin-5](https://github.com/JamesErvin-5)
  * [readme-ru.md]
  * [quickstart-ru.md]
* Update
  * add header, give credit
    * [en-us.cfg] v1.1.3.0
    * [es-es.cfg] v1.1.3.0
    * [es-mx.cfg] v1.1.3.0
    * [ru.cfg] v1.1.3.0
  * [quickstart.md]
  * [readme.md]
* closes #43 - Localization - Mexican (Mexicano) <es-mx.cfg>
* updates #47 - Localization - Master

### Status 1.6.4.0

* Issues
  * closes #71 - The Gold Standard (GOLD) 1.6.4.0-release `<Thank you Dewar>` edition
  * closes #72 - 1.6.4.0 Additional Tasks
  * closes #69 - Update The Gold Standard (GOLD)
  * updates #8 - 'Stockalike' textures
  * updates #7 - B9 Tank Switch
  * updates #53 - Maybe a third ore like palladium
  * updates #50 - Near Future Construction (NFC) Compatibility
  * updates #49 - Station Parts Expansion Redux (SSPx) Compatibility

---

## Version 1.6.3.0 - `<Gold Pans ReStocked>`

* 22 Jan 2022
* Released for Kerbal Space Program 1.12.3

### Updated ♻ 1.6.3.0

* renamed /Patches --> Compatibility

### CargoPart Review

* volume review (math shown below)
* game volume is in Liters (L)
* closes #48 - Review CargoPart
* small (1.25m) tanks had their cargo volumes reduced a small amount

#### Math

  | Ore Tanks    |            |           |            | πr²h    | 1000L = m3 |
  | ------------ | ---------- | --------- | ---------- | ------- | ---------- |
  | diameter (m) | radius (m) | height(m) | volume m^3 | *1000   |
  | large        | 2.5        | 1.25      | 1.9000     | 9.3266  | 9326.61    |
  | small        | 1.25       | 0.625     | 1.9000     | 2.33165 | 2331.66    |
  | radial       | 0.625      | 0.3125    | 1.0000     | 0.3068  | 306.8      |
  
### missing drag cubes

* closes #54 -  LargeGoldTank and LargeGoldOreTank missing drag cube

### Linting  and file maintenance :deciduous_tree:

* all part.cfg's
* add Dewar and zer0Kerbal to authors
* minor housekeeping  
* patch dusting (mostly removing construction dust (comments)) 

### Squad-Tanks patches

* rename [Squad.cfg] to [Squad-Tanks.cfg] 1.2.0.0
* add [ModuleCargoPart] to all
  * Radial: 340 (already there)
  * Small: 2350
  * Large: 9500
* update patch license
* closes #55 - Squad-Tank patches

### Squad patches

* rename [Patches.cfg] to [Squad.cfg] 1.2.0.0
* remove sneaky little `MODULE[ModuleResourceHarvester]`
* Undo localization on some items
  * ResourceName
  * resourceName
* update patch license
* closes #56 - Squad patches

### Update [StockalikeMiningExpansion.cfg] v1.1.1.0

* update patch license

### Update [SCANSat.cfg] 1.1.0.2

* rename [Scansat.cfg] to [SCANSat.cfg] 1.1.0.2
* update patch license
* linting

### Add Restock.restockwhitelist

* closes #6 - ReStock compliance
* closes #58 - Add Restock.restockwhitelist

### RadialTank packedVolume

* currently is packedVolume = 325
* stock is packedVolume = 340
* change to equal stock
* closes #57 - RadialTank packedVolume

### Status 1.6.3.0

* Localizations
  * closes #44 - Localization - Spanish (Español) <es-es.cfg> - thank you Fitiales
  * closes #65 - Localization - Russian (Русский) <ru.cfg> - thank you to DirtyThongSniffer
* Issues 
  * updates #47 - us-en.cfg should be complete
  * closes #46 - Localization - English (United States)] <en-us.cfg>
  * closes - #60 - Version 1.6.3.0-release
  * closes - #61 - 1.6.3.0 Legal MumboJumbo
  * closes - #62 - 1.6.3.0 Update documentation
  * closes - #63 - Release 1.6.3.0-release
  * closes - #64 - 1.6.3.0 Social Media
* Bug
  * closes #5 - Tank costs 
  * closes #12 - Text issue with SMX - anything remaining isn't a Localization issue
  * closes #15 - Drill patches need updating?
  * closes #16 - Tanks ModuleCargoPart: packedVolume
  * updates #11 - us-en.cfg should be complete
  * closes #27 - Empty Ore Tanks result in Negative Funds Career Mode

---

## Version 1.6.2.1 - 2022-01-23 [KSP 1.12.2]

### Status 1.6.2.1

* Issues 
  * closes #20 - `TheGoldStandard.version` :congratulations: bug -  contributed by zer0Kerbal
  * closes #23 - Localization - zh-cn.cfg - Simplified Chinese duplicate
  * closes #24 - Localization - pt-br.cfg Brazil duplicate
  * closes #25 - Localization - en-us.cfg (English) duplicate
  * closes #26 - Localization - duplicate
  * closes #28 - Localization - [Taiwanese (国语))][TW] <zh-tw.cfg>   duplicate
  * closes #29 - Localization - [Simplified Chinese (简体中文))][CN] <zh-cn.cfg>  duplicate
  * closes #30 - Localization - [Swedish (Svenska)][SW] <sw-sw.cfg>    duplicate
  * closes #51 - Add es-es.cfg- contributed by Fitiales
  * closes #52 - Localization - Russian (Русский) <ru.cfg> - contributed by zer0Kerbal
  * closes #60 - Version 1.6.3.0-release
  * closes #61 - 1.6.3.0 Legal MumboJumbo
  * closes #62 - 1.6.3.0 Update documentation
  * closes #63 - Release 1.6.3.0-release
  * closes #64 - 1.6.3.0 Social Media
* Bug
  * closes #5 - Tank costs 
  * closes #12 - Text issue with SMX - anything remaining isn't a Localization issue
  * closes #15 - Drill patches need updating?
  * closes #16 - Tanks ModuleCargoPart: packedVolume
  * closes #11 - Localization  duplicate
  * closes #46 - Localization - English (United States)] <en-us.cfg>
  * updates #47 - us-en.cfg should be complete

---

## Version 1.6.0.0 - `<Eureka!>`

* Version 1.6.2.0 - 2021-09-15 [KSP 1.12.2]
* Version 1.6.0.0-prerelease - 2021-07-25 [KSP 1.12.2]

* 2021-06-27
* For KSP  1.11.2

### Release 1.6.0.0

* for KSP 1.11.2
* should be last release for 1.11.2

### Correction 1.6.0.0

* Gold Smelter localization tags
  * they were tagged with an extra '-'
  * Thank you to @TheKurgan for finding the following:

### Updated 1.6.0.0

* SCANSat.cfg
  * renamed SCANSat.cfg -> SCANsat.cfg
  * SCANSAT-SENSOR -> SCANSAT_SENSOR
* GoldOre.cfg
  * PLANETARY_RESOURCE -> PLANETARY_RESOURCE
  * GLOBAL-RESOURCE _> GLOBAL_RESOURCE
* Unobtainium.cfg 
  * Split out from GoldOre.cfg
* GoldSmelter.cfg and Patches.cfg
  * INPUT-RESOURCE -> INPUT_RESOURCE
  * OUTPUT-RESOURCE -> OUTPUT_RESOURCE
  *oldSmelter.cfg
  * STAGE_PRIORITY_FLOW -> STAGE_PRIORITY_FLOW
    * ResouceGeneric.cfg: 'ALL-VESSEL' when should be 'ALL_VESSEL'
* Cargo Pass
  * added ModuleCargoPart
* part.cfg pass
  * fully updated and modernized all parts
  * added @thumbs
  * added ModuleFuelJettison
  * added DragCubes
* resource.cfg's
  * fully updated and modernized all resource definitions
* Thanks to @Dewar and @HebaruSan and @Skall
  * SpaceDock is now updated
  * CKAN is now updated and unfrozen.

### NEW - but not included 1.6.0.0

* PartVariants
  * by popular demand, you can now select one of two part variant themed skins for the tanks. The default is The Gold Standard, pun intended; or you can choose stock. Can't get more stock-alike 
  * the hold up is have to account for ReStock.
  * Enterprising players will figure something out.

### Added 1.6.0.0

* Stockalike Mining Expansion (SMX)
  * added StockalikeMiningExpansion.cfg
  * converted to use Localization strings
  * based upon @TheProtagonists version https://forum.kerbalspaceprogram.com/index.php?/topic/130325-110x-stockalike-mining-extension-115-release-782020/&do=findComment&comment=3203456
* GoldSmelter
  * added resources: ElectricCharge (100,10), Gold (0,5), GoldOre (0,5)
  
### Localization 1.6.0.0

* Localization
  * us-en.cfg should be completed
  * added localization.md

### Adoption 1.6.0.0

* -- Adoption by zer0Kerbal --
  * Restructure folders
  * moved models/textures into /Assets/
  * moved patches into /Patches/
  * initial Localization push
  * created GitHub Repo
  * created Curseforge page
  * created new forum thread
  * removed included Module Manager
  * updated to automated backend processes.
  * linting and duct taping

### Status 1.6.0.0

* closes 4 - bunch of errors where a - was used instead of an _ bug
* closes 9 - 1.6.1.0 - Underscored for KSP 1.12.1 (07 Aug 2021) bug - contributed by zer0Kerbal
* closes 17 - 1.6.2.0 overpriced bug - contributed by zer0Kerbal
* closes 18 - 1.6.2.0 overpriced - contributed by zer0Kerbal
* closes #1 - capturing upstream changes - contributed by zer0Kerbal
* closes 2 - 1.6.0.0 adoption - contributed by zer0Kerbal

---

## Version 1.5.2

* Packaged the latest version of MM to bring the mod upto 1.3

---

## Version  1.5.1  

* Complete Compatibility with SCANsat and Galileo's Planet Pack  
* Changed the way resources spawn on planets (more small concentrated veins, less large low concentrated blobs)

---

## Version  1.5 -  Thanks go to Jadeofmaar for helping me here

* Improved Weight/Balance/Distribution of resources. It should now be a little easier to make money, and more worth it to make a trip out farther.
* Fixed the Unobtainium texture
* Cleaned up files
* Improved compatibility with SCANSat and Galileo's Planet Pack

---

## Version  1.4.2

* Fixed stupid typo ftw

---

## Version  1.4.1

* Fixed a value that was preventing Unobtainium from spawning in large enough quantities to be mined

---

## Version  1.4

* Finally got of my butt and updated the mod to 1.2.2
* Added Unobtainium 
* Added support for GPP and SCANSat

---

## Version  1.3 

* Updated to for KSP 1.2 
* Fixed a potential problem with unlimited output for both gold smeltery and stock miniISRUVersion 1

---

## Version  1.2

* Updated some part descriptions
* Slightly reduced concentrations of gold on Minmus
* Made orbital scanner unlock earlier (The satellite targeting gui is disabled until survey scan)
* Adjusted Smeltery Output to prevent a very minor exploit

---

## Version  1.1

* Cleaned up textures
* Fixed radial attachment points
* Added Mission Flags

---

## Version  1.0

* 01 Oct 2016
* Release

### CC BY-NC-ND 3.0 Unported by zer0Kerbal