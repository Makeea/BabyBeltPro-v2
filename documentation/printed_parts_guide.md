# BabyBelt Pro V2 Printed Parts List
BabyBelt Pro V2 by RobMink

## Introduction
Hello! This is the printed parts guide for the BabyBelt Pro V2 by RobMink. 

How to read this guide:
 - Printed Parts will link to the specific file in the GitHub if clicked on
 - Printed part name prefixes include
   - [a] = accent color
   - [s] = needs supports
   - [i] = needs heat-set inserts
   - [HT] = should be printed in a strong heat tolerant material (PETG, ABS, ASA, PA) to avoid premature wearing

## Printed Parts
### Printing Parts
Most of the parts of this kit can be printed out of normal PLA, allowing for a wide range of colors and stylistic choices! The parts that shouldn't be printed out of PLA are listed below. A good rule of thumb is if you only ever plan to print PLA or TPU, your Bed/Underbed can be PETG. However, if printing in PETG, it is **HIGHLY** suggested to use ABS or ASA. 

- [*NEMA17_ZGear*](../STLs/ZBeltDrive/[a]_BBProV25fl_Nema17_ZGear.stl)
- [*Roller_ZGear*](../STLs/ZBeltDrive/[a]_BBProV25fl_Roller_ZGear.stl)
- [*UnderbedOrBed*](../STLs/ZBeltDrive/[HT]_BBProV25fl_UnderbedOrBed.stl)

We recommend printing all parts with standard Voron style settings:

- Layer height: 0.2mm
- Extrusion width: 0.4mm, forced
- Infill percentage: 40%
- Infill type: grid, gyroid, honeycomb, triangle, or cubic
- Wall count: 4, use 5 walls on [[a,s]_BBProV25fl_Roller[x2]](../STLs/ZBeltDrive/[a,s]_BBProV25fl_Roller[x2].stl)
- Solid top/bottom layers: 5

### Bambu Studio Project Files (3MF)
Ready-to-slice Bambu Studio projects are included for each group of parts. The STL files above and in the part list below are unchanged, so use those if you have a different printer or slicer.

The projects are set up for two printers, both with a 0.4mm nozzle and the High Temp Plate. Parts that can be PLA print in PLA on a Bambu Lab A1. Parts that need a stronger, heat tolerant material print in ASA on a Bambu Lab P1S, which has an enclosure. All projects use the settings recommended above:

- Layer height: 0.2mm
- Line width: 0.4mm on every line type, including the first layer
- Infill: 40% grid
- Walls: 4 (5 on the rollers)
- Top/bottom layers: 5
- Supports: only on [s] parts (tree, auto)
- Brim: none

|Project|Printer|Material|Plates|Parts|
|-----|-----|-----|-----|-----
|[BBPro_Frame](../STLs/Frame/BBPro_Frame.3mf)|A1|PLA|2|Side-A + Side-B; scraper + Screenmount (supports)
|[BBPro_GantryY](../STLs/Gantry/Y/BBPro_GantryY.3mf)|A1|PLA|1|Tensioner body, idler holder, tensioner nut, LinearRailReplacement V26, LDO toolboard mount
|[BBPro_GantryX](../STLs/Gantry/X/BBPro_GantryX.3mf)|A1|PLA|1|X-Carraige, motor mount, Xrail mounts A/B, Xrail under-mounts A/B, pivot arm (2x), X pivot clamp (2x)
|[BBPro_Carriage_Bambu](../STLs/Gantry/Carriage/Bambu/BBPro_Carriage_Bambu.3mf)|A1|PLA|1|YCar SideA (V26), SideB, BeltHolder, Fan
|[BBPro_PrintBelt](../STLs/PrintBelt/BBPro_PrintBelt.3mf)|A1|PLA|1|Frame-A/B, Nut (2x), Pusher-A/B
|[BBPro_ZBeltDrive_Rollers_PLA](../STLs/ZBeltDrive/BBPro_ZBeltDrive_Rollers_PLA.3mf)|A1|PLA|1|Rollers (2x, 5 walls, supports)
|[BBPro_ZBeltDrive_ASA](../STLs/ZBeltDrive/BBPro_ZBeltDrive_ASA.3mf)|P1S|ASA|1|LDO heatbed underbed, Roller_ZGear, Nema17_ZGear (2x)

Filament in the projects:

- PLA projects (A1) use Ambrosia PLA: 210°C nozzle (range 190-220°C), 60°C bed, part cooling fan at Bambu's PLA default.
- The ASA project (P1S) holds the parts the guide says should not be PLA: the Z gears (PETG or stronger) and the LDO heatbed underbed (heat tolerant). The underbed sits directly under the heater, so PETG is avoided there because it softens at around 70-80°C. The project uses iSANGHU ASA: 270°C nozzle (range 260-280°C), 100°C bed (the P1S maximum), part cooling fan 10-40%, auxiliary fan off. If you use a different ASA, select its profile in Bambu Studio before slicing.
- A plate can only have one bed temperature, so PLA and ASA parts are kept in separate projects.

Filaments used:

|Filament|Used for|Store|Manufacturer|Profile|
|-----|-----|-----|-----|-----
|Ambrosia PLA, Rainbow Rush, 1kg|PLA projects (A1)|[West3D](https://west3d.com/products/ambrosia-pla-filament-of-the-gods-1kg-bambu-ams-friendly-cardboard-spools-premium-3d-printing-filament?variant=46039719018708) (not found on Amazon)|[Ambrosia Filament](https://ambrosiafilament.com/products/ambrosia-pla-filament-of-the-gods-1kg-bambu-ams-friendly-cardboard-spools-premium-3d-printing-filament?variant=50588085027130)|[3D Filament Profiles](https://3dfilamentprofiles.com/filament/details/4468)
|iSANGHU ASA, Emerald Wave, 1kg|ASA project (P1S)|[Amazon](https://www.amazon.com/dp/B0DCSQ6ZZM)|[iSANGHU on Amazon](https://www.amazon.com/3D-Printing-Filament-iSANGHU-Supplies/s?keywords=3D+Printing+Filament&rh=n:6066129011,p_89:iSANGHU&c=ts&ts_id=6066129011) (no official manufacturer site found)|[3D Filament Profiles](https://3dfilamentprofiles.com/defaults/isanghu/asa/basic)

Printing tips:

- PLA on the A1: no special steps. If printing PLA on the P1S instead, prop the lid open to avoid heat creep.
- ASA on the P1S: keep the lid and door closed, let the bed heat the chamber for about 10 minutes before printing, use glue stick on the plate, and print in a ventilated area.
- Large flat parts (frame sides, underbed) can lift at the corners. If they do, add a brim to just that part.
- Check that each part lies flat on the plate before slicing. Bambu Studio may reset the print or filament settings to its saved presets when a project is saved, so confirm the settings above are still in place before printing.
- Parts marked [i] (X-Carraige, Xrail under-mounts) need heat-set inserts after printing.


## Part List
|Name|Image|Area|Color|Supports|Heat-Sets|Material|Description
|-----|-----|-----|-----|-----|-----|-----|-----
|[BBProV25fl_scraper](../STLs/Frame/BBProV25fl_scraper.stl)|![BBProV25fl_scraper](./images/printed_parts/Frame/BBProV25fl_scraper.jpg)|Frame|Main|No|No|>= PLA|
|[BBProV25fl_Side-A](../STLs/Frame/BBProV25fl_Side-A.stl)|![BBProV25fl_Side-A](./images/printed_parts/Frame/BBProV25fl_Side-A.jpg)|Frame|Main|No|No|>= PLA|
|[BBProV25fl_Side-B](../STLs/Frame/BBProV25fl_Side-B.stl)|![BBProV25fl_Side-B](./images/printed_parts/Frame/BBProV25fl_Side-B.jpg)|Frame|Main|No|No|>= PLA|
|[[s]_BBProV24fl_Screenmount](../STLs/Frame/[s]_BBProV24fl_Screenmount.stl)|![[s]_BBProV24fl_Screenmount](./images/printed_parts/Frame/[s]_BBProV24fl_Screenmount.jpg)|Frame|Main|Yes|No|>= PLA|
|[[a]_BBProV25fl_YCar_Bam_BeltHolder](../STLs/Gantry/Carriage/Bambu/[a]_BBProV25fl_YCar_Bam_BeltHolder.stl)|![[a]_BBProV25fl_YCar_Bam_BeltHolder](./images/printed_parts/Gantry/Carriage/Bambu/[a]_BBProV25fl_YCar_Bam_BeltHolder.jpg)|Gantry/Carriage/Bambu|Accent|No|No|>= PLA|
|[[a]_BBProV25fl_YCar_Bam_Fan](../STLs/Gantry/Carriage/Bambu/[a]_BBProV25fl_YCar_Bam_Fan.stl)|![[a]_BBProV25fl_YCar_Bam_Fan](./images/printed_parts/Gantry/Carriage/Bambu/[a]_BBProV25fl_YCar_Bam_Fan.jpg)|Gantry/Carriage/Bambu|Accent|No|No|>= PLA|
|[[a]_BBProV25fl_YCar_Bam_SideB](../STLs/Gantry/Carriage/Bambu/[a]_BBProV25fl_YCar_Bam_SideB.stl)|![[a]_BBProV25fl_YCar_Bam_SideB](./images/printed_parts/Gantry/Carriage/Bambu/[a]_BBProV25fl_YCar_Bam_SideB.jpg)|Gantry/Carriage/Bambu|Accent|No|No|>= PLA|
|[[a]_BBProV26fl_YCar_Bam_SideA](../STLs/Gantry/Carriage/Bambu/[a]_BBProV26fl_YCar_Bam_SideA.stl)|![[a]_BBProV26fl_YCar_Bam_SideA](./images/printed_parts/Gantry/Carriage/Bambu/[a]_BBProV26fl_YCar_Bam_SideA.jpg)|Gantry/Carriage/Bambu|Accent|No|No|>= PLA|
|[[i]_BBProV26fl_X-Carraige](../STLs/Gantry/X/[i]_BBProV26fl_X-Carraige.stl)|![[i]_BBProV26fl_X-Carraige](./images/printed_parts/Gantry/X/[i]_BBProV26fl_X-Carraige.jpg)|Gantry/X|Main|No|Yes|>= PLA|
|[BBProV26fl_X-CarraigeMotorMount](../STLs/Gantry/X/BBProV26fl_X-CarraigeMotorMount.stl)|![BBProV26fl_X-CarraigeMotorMount](./images/printed_parts/Gantry/X/BBProV26fl_X-CarraigeMotorMount.jpg)|Gantry/X|Main|No|No|>= PLA|
|[[a]_BBProV25fl_pivotArm(2x)](../STLs/Gantry/X/[a]_BBProV25fl_pivotArm(2x).stl)|![[a]_BBProV25fl_pivotArm(2x)](./images/printed_parts/Gantry/X/[a]_BBProV25fl_pivotArm(2x).jpg)|Gantry/X|Accent|No|No|>= PLA|
|[[a]_BBProV25fl_XPivotClamp(2x)](../STLs/Gantry/X/[a]_BBProV25fl_XPivotClamp(2x).stl)|![[a]_BBProV25fl_XPivotClamp(2x)](./images/printed_parts/Gantry/X/[a]_BBProV25fl_XPivotClamp(2x).jpg)|Gantry/X|Accent|No|No|>= PLA|
|[[a]_BBProV26fl_XrailMount-SideA](../STLs/Gantry/X/[a]_BBProV26fl_XrailMount-SideA.stl)|![[a]_BBProV26fl_XrailMount-SideA](./images/printed_parts/Gantry/X/[a]_BBProV26fl_XrailMount-SideA.jpg)|Gantry/X|Accent|No|No|>= PLA|
|[[a]_BBProV26fl_XrailMount-SideB](../STLs/Gantry/X/[a]_BBProV26fl_XrailMount-SideB.stl)|![[a]_BBProV26fl_XrailMount-SideB](./images/printed_parts/Gantry/X/[a]_BBProV26fl_XrailMount-SideB.jpg)|Gantry/X|Accent|No|No|>= PLA|
|[[ai]_BBProV26fl_XrailMountUnder-SideA](../STLs/Gantry/X/[ai]_BBProV26fl_XrailMountUnder-SideA.stl)|![[ai]_BBProV26fl_XrailMountUnder-SideA](./images/printed_parts/Gantry/X/[ai]_BBProV26fl_XrailMountUnder-SideA.jpg)|Gantry/X|Accent|No|Yes|>= PLA|
|[[ai]_BBProV26fl_XrailMountUnder-SideB](../STLs/Gantry/X/[ai]_BBProV26fl_XrailMountUnder-SideB.stl)|![[ai]_BBProV26fl_XrailMountUnder-SideB](./images/printed_parts/Gantry/X/[ai]_BBProV26fl_XrailMountUnder-SideB.jpg)|Gantry/X|Accent|No|Yes|>= PLA|
|[BBProV25fl_RockMonsterNo1YTentionerNut](../STLs/Gantry/Y/BBProV25fl_RockMonsterNo1YTentionerNut.stl)|![BBProV25fl_RockMonsterNo1YTentionerNut](./images/printed_parts/Gantry/Y/BBProV25fl_RockMonsterNo1YTentionerNut.jpg)|Gantry/Y|Main|No|No|>= PLA|
|[BBProV26fl_LinearRailReplacement](../STLs/Gantry/Y/BBProV26fl_LinearRailReplacement.stl)|![BBProV26fl_LinearRailReplacement](./images/printed_parts/Gantry/Y/BBProV26fl_LinearRailReplacement.jpg)|Gantry/Y|Main|No|No|>= PLA|
|[LDO Kit - Toolboard Mount v1](../STLs/Gantry/Y/LDO%20Kit%20-%20Toolboard%20Mount%20v1.stl)|![LDO Kit - Toolboard Mount v1](./images/printed_parts/Gantry/Y/LDO%20Kit%20-%20Toolboard%20Mount%20v1.jpg)|Gantry/Y|Main|No|No|>= PLA|
|[[a]_BBProV25fl_RockMonsterNo1YTentionerIdlerHolder](../STLs/Gantry/Y/[a]_BBProV25fl_RockMonsterNo1YTentionerIdlerHolder.stl)|![[a]_BBProV25fl_RockMonsterNo1YTentionerIdlerHolder](./images/printed_parts/Gantry/Y/[a]_BBProV25fl_RockMonsterNo1YTentionerIdlerHolder.jpg)|Gantry/Y|Accent|No|No|>= PLA|
|[[a]_BBProV26fl_RockMonsterNo1YTentionerBody](../STLs/Gantry/Y/[a]_BBProV26fl_RockMonsterNo1YTentionerBody.stl)|![[a]_BBProV26fl_RockMonsterNo1YTentionerBody](./images/printed_parts/Gantry/Y/[a]_BBProV26fl_RockMonsterNo1YTentionerBody.jpg)|Gantry/Y|Accent|No|No|>= PLA|
|[[a]_BBProV25fl_PrintBelt-Frame-A](../STLs/PrintBelt/[a]_BBProV25fl_PrintBelt-Frame-A.stl)|![[a]_BBProV25fl_PrintBelt-Frame-A](./images/printed_parts/PrintBelt/[a]_BBProV25fl_PrintBelt-Frame-A.jpg)|PrintBelt|Accent|No|No|>= PLA|
|[[a]_BBProV25fl_PrintBelt-Frame-B](../STLs/PrintBelt/[a]_BBProV25fl_PrintBelt-Frame-B.stl)|![[a]_BBProV25fl_PrintBelt-Frame-B](./images/printed_parts/PrintBelt/[a]_BBProV25fl_PrintBelt-Frame-B.jpg)|PrintBelt|Accent|No|No|>= PLA|
|[[a]_BBProV25fl_PrintBelt-Nut(2x)](../STLs/PrintBelt/[a]_BBProV25fl_PrintBelt-Nut(2x).stl)|![[a]_BBProV25fl_PrintBelt-Nut(2x)](./images/printed_parts/PrintBelt/[a]_BBProV25fl_PrintBelt-Nut(2x).jpg)|PrintBelt|Accent|No|No|>= PLA|
|[[a]_BBProV25fl_PrintBelt-Pusher-A](../STLs/PrintBelt/[a]_BBProV25fl_PrintBelt-Pusher-A.stl)|![[a]_BBProV25fl_PrintBelt-Pusher-A](./images/printed_parts/PrintBelt/[a]_BBProV25fl_PrintBelt-Pusher-A.jpg)|PrintBelt|Accent|No|No|>= PLA|
|[[a]_BBProV25fl_PrintBelt-Pusher-B](../STLs/PrintBelt/[a]_BBProV25fl_PrintBelt-Pusher-B.stl)|![[a]_BBProV25fl_PrintBelt-Pusher-B](./images/printed_parts/PrintBelt/[a]_BBProV25fl_PrintBelt-Pusher-B.jpg)|PrintBelt|Accent|No|No|>= PLA|
|[[a,s]_BBProV25fl_Roller[x2]](../STLs/ZBeltDrive/[a,s]_BBProV25fl_Roller[x2].stl)|![[a,s]_BBProV25fl_Roller[x2]](./images/printed_parts/ZBeltDrive/[a,s]_BBProV25fl_Roller[x2].jpg)|ZBeltDrive|Accent|Yes|No|>= PLA|
|[[a]_BBProV25fl_Nema17_ZGear](../STLs/ZBeltDrive/[a]_BBProV25fl_Nema17_ZGear.stl)|![[a]_BBProV25fl_Nema17_ZGear](./images/printed_parts/ZBeltDrive/[a]_BBProV25fl_Nema17_ZGear.jpg)|ZBeltDrive|Accent|No|No|>= PETG|
|[[a]_BBProV25fl_Roller_ZGear](../STLs/ZBeltDrive/[a]_BBProV25fl_Roller_ZGear.stl)|![[a]_BBProV25fl_Roller_ZGear](./images/printed_parts/ZBeltDrive/[a]_BBProV25fl_Roller_ZGear.jpg)|ZBeltDrive|Accent|No|No|>= PETG|
|[[HT]_BBProV25fl_Underbed-notforbed-FOR_LDO_HEATBED](../STLs/ZBeltDrive/[HT]_BBProV25fl_Underbed-notforbed-FOR_LDO_HEATBED.stl)|![[HT]_BBProV25fl_Underbed-notforbed-FOR_LDO_HEATBED](./images/printed_parts/ZBeltDrive/[HT]_BBProV25fl_Underbed-notforbed-FOR_LDO_HEATBED.jpg)|ZBeltDrive|Main|No|No|>= PETG| Use this when installing LDO bed heater.
|[[HT]_BBProV25fl_UnderbedOrBed](../STLs/ZBeltDrive/[HT]_BBProV25fl_UnderbedOrBed.stl)|![[HT]_BBProV25fl_UnderbedOrBed](./images/printed_parts/ZBeltDrive/[HT]_BBProV25fl_UnderbedOrBed.jpg)|ZBeltDrive|Main|No|No|>= PETG| Use this for no heated bed.
