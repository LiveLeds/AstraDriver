---
layout: home
---

{% assign cacheBust = site.time | date:'?v=%s' %}
![Image]({{ "/images/AstraDriver-3D_blender_top_angled.png" | relative_url | append: cacheBust }}){: width="400" }

ESP32-based control PCB uses WiFi with an external antenna and 5Mbps RS-485
for communication, supporting various sensors and HMI devices for high-power 
LED fixtures or strips. One device can act as master or all fixtures will receive 
data from a dedicated receiver.


[![CI](https://github.com/alexanderp4580/astra-control-pcb/actions/workflows/ci.yml/badge.svg)](https://github.com/alexanderp4580/astra-control-pcb/actions/workflows/ci.yml)
## Table of contents

- [Table of contents](#table-of-contents)
  - [Render Top Angled](#render-top-angled)
  - [Render Top](#render-top)
  - [Render Bottom](#render-bottom)
  - [Interactive BOM](#interactive-bom)
  - [BOM](#bom)
  - [KiCad Revision Inspector (KiRI)](#kicad-revision-inspector-kiri)
    - [Dark](#dark)
    - [Light](#light)
  - [Schematic](#schematic)
    - [Dark](#dark-1)
    - [Monochromatic](#monochromatic)
    - [Light](#light-1)
  - [Assembly](#assembly)
    - [Dark](#dark-2)
    - [Light](#light-2)
  - [Downloads](#downloads)
    - [JLCPCB](#jlcpcb)
    - [Eurocircuits](#eurocircuits)
- [Report](#report)
    - [ERC](#erc)
    - [DRC](#drc)
- [Credits](#credits)

### Render Top Angled

![Image]({{ "/images/AstraDriver-3D_blender_top_angled.png" | relative_url | append: cacheBust }})

### Render Top

![Image]({{ "/images/AstraDriver-3D_blender_top.png" | relative_url | append: cacheBust }})

### Render Bottom

![Image]({{ "/images/AstraDriver-3D_blender_bottom.png" | relative_url | append: cacheBust }})

### Interactive BOM

Easily check component locations by hovering over a specific component.

[IBOM HTML]({{ "/export/AstraDriver-ibom.html" | relative_url | append: cacheBust }})

### BOM

All components with Values, References, Sheetpath and Links to the datasheet.

[BOM HTML]({{ "/export/AstraDriver-bom.html" | relative_url | append: cacheBust }})

### KiCad Revision Inspector (KiRI)

KiCad Revision Inspector (KiRI) is a tool for comparing different versions of KiCad projects. It exports project revisions to SVG format for visual comparison using an onion skin view. This helps identify changes and errors in PCB designs. KiRI also includes a command line interface for generating viewable artifacts in any web browser.

View the PCB / Schematic in an interactive way, pan and zoom to see the details.

#### Dark

- [KiRi Dark]({{ "/KiRiDark/index.html" | relative_url | append: cacheBust }})

#### Light

- [KiRi Light]({{ "/KiRiLight/index.html" | relative_url | append: cacheBust }})

### Schematic

#### Dark

- [Schematic Dark PDF]({{ "/documents/AstraDriver-schematic-dark.pdf" | relative_url | append: cacheBust }})

#### Monochromatic

- [Schematic Monochromatic PDF]({{ "/documents/AstraDriver-schematic-mono.pdf" | relative_url | append: cacheBust }})

#### Light

- [Schematic Light PDF]({{ "/documents/AstraDriver-schematic-default.pdf" | relative_url | append: cacheBust }})

### Assembly

#### Dark

- [PCB Dark PDF]({{ "/documents/AstraDriver-pcb-dark.pdf" | relative_url | append: cacheBust }})

#### Light

- [PCB Light PDF]({{ "/documents/AstraDriver-pcb-light.pdf" | relative_url | append: cacheBust }})

### Downloads

#### JLCPCB

- [JLCPCB Zip]({{ "export/AstraDriver-JLCPCB.zip" | relative_url | append: cacheBust }})
- [JLCPCB BOM CSV]({{ "export/AstraDriver_bom_jlc.csv" | relative_url | append: cacheBust }})
- [JLCPCB CPL CSV]({{ "export/AstraDriver_cpl_jlc.csv" | relative_url | append: cacheBust }})

#### Eurocircuits

- [Eurocircuits Zip]({{ "export/AstraDriver-Eurocircuits.zip" | relative_url | append: cacheBust }})
- [Eurocircuits BOM CSV]({{ "export/AstraDriver_bom_Eurocircuits.csv" | relative_url | append: cacheBust }})
- [Eurocircuits CPL CSV]({{ "export/AstraDriver_cpl_Eurocircuits.csv" | relative_url | append: cacheBust }})
  
## Report

#### ERC

{% include_relative erc_validation.md %}

#### DRC

{% include_relative drc_validation.md %}

{% include_relative AstraDriver-report.md %}


## Credits

[KiCad EDA](https://www.kicad.org)

[KiBot](https://github.com/INTI-CMNB/KiBot)

[Amulet - Inspiration for awesome schematic and PCB](https://github.com/EPFLXplore/XRE_LeggedRobot_HW)

Sorry if I am forgetting someone, I used lots of references and tips from all over the place.