---
layout: home
---

{% assign cacheBust = site.time | date:'?v=%s' %}
![Image]({{ "/images/AstraDriver-3D_blender_top_angled.png" | absolute_url | append: cacheBust }}){: width="400" }

4 Channel LED Driver with PWM dimming input. LED2001PHR is the driver IC, 
it can support up to 4A, 3V - 18V at 850KHz switching frequency.
Test plugs for each input and output.
Optimized for good dimming performance.

[![CI](https://github.com/LiveLeds/AstraDriver/actions/workflows/ci.yml/badge.svg)](https://github.com/LiveLeds/AstraControl/actions/workflows/ci.yml)

![GitHub last commit](https://img.shields.io/github/last-commit/liveleds/AstraDriver?link=https%3A%2F%2Fgithub.com%2FLiveLeds%2FAstraDriver)

## Table of contents

- [Table of contents](#table-of-contents)
  - [Render Top Angled](#render-top-angled)
  - [Render Top](#render-top)
  - [Render Bottom](#render-bottom)
  - [Schematic](#schematic)
    - [Dark](#dark)
    - [Monochromatic](#monochromatic)
    - [Light](#light)
  - [Assembly](#assembly)
    - [Dark](#dark-1)
    - [Light](#light-1)
    - [Gerber viewer on tracespace.io](#gerber-viewer-on-tracespaceio)
  - [Interactive BOM](#interactive-bom)
  - [BOM](#bom)
  - [KiCad Revision Inspector (KiRI)](#kicad-revision-inspector-kiri)
    - [Dark](#dark-2)
    - [Light](#light-2)
  - [Downloads](#downloads)
    - [JLCPCB](#jlcpcb)
    - [Eurocircuits](#eurocircuits)
    - [3D Step](#3d-step)
- [Report](#report)
    - [ERC](#erc)
    - [DRC](#drc)
- [Know Issues](#know-issues)
- [Credits](#credits)

### Render Top Angled

![Image]({{ "/images/AstraDriver-3D_blender_top_angled.png" | absolute_url | append: cacheBust }})

### Render Top

![Image]({{ "/images/AstraDriver-3D_blender_top.png" | absolute_url | append: cacheBust }})

### Render Bottom

![Image]({{ "/images/AstraDriver-3D_blender_bottom.png" | absolute_url | append: cacheBust }})

### Schematic

#### Dark

- [Schematic Dark PDF]({{ "/documents/AstraDriver-schematic-dark.pdf" | absolute_url | append: cacheBust }})

#### Monochromatic

- [Schematic Monochromatic PDF]({{ "/documents/AstraDriver-schematic-mono.pdf" | absolute_url | append: cacheBust }})

#### Light

- [Schematic Light PDF]({{ "/documents/AstraDriver-schematic-default.pdf" | absolute_url | append: cacheBust }})

### Assembly

#### Dark

- [PCB Dark PDF]({{ "/documents/AstraDriver-pcb-dark.pdf" | absolute_url | append: cacheBust }})

#### Light

- [PCB Light PDF]({{ "/documents/AstraDriver-pcb-light.pdf" | absolute_url | append: cacheBust }})

#### Gerber viewer on tracespace.io

[https://tracespace.io/view/?boardUrl={{ "export/AstraDriver-JLCPCB.zip" | absolute_url | append: cacheBust }}](https://tracespace.io/view/?boardUrl={{ "export/AstraDriver-JLCPCB.zip" | absolute_url | append: cacheBust }})

### Interactive BOM

Check component locations by hovering over a specific component.
The visual elements might not be precise enough for pcb review but can be very useful since it's possible to pan and zoom.
Not all BOM columns are available here, for datasheet links see BOM below.

[IBOM HTML]({{ "/export/AstraDriver-ibom.html" | absolute_url | append: cacheBust }})

### BOM

All components with Values, References, Sheetpath and Links to the datasheet.

[BOM HTML]({{ "/export/AstraDriver-bom.html" | absolute_url | append: cacheBust }})

### KiCad Revision Inspector (KiRI)

KiCad Revision Inspector (KiRI) is a tool for comparing different versions of KiCad projects. It exports project revisions to SVG format for visual comparison using an onion skin view. This helps identify changes and errors in PCB designs. KiRI also includes a command line interface for generating viewable artifacts in any web browser.

View the PCB / Schematic in an interactive way, pan and zoom to see the details.

#### Dark

- [KiRi Dark]({{ "/KiRiDark/index.html" | absolute_url | append: cacheBust }})

#### Light

- [KiRi Light]({{ "/KiRiLight/index.html" | absolute_url | append: cacheBust }})

### Downloads

#### JLCPCB

- [JLCPCB Zip]({{ "export/AstraDriver-JLCPCB.zip" | absolute_url | append: cacheBust }})
- [JLCPCB BOM CSV]({{ "export/AstraDriver_bom_jlc.csv" | absolute_url | append: cacheBust }})
- [JLCPCB CPL CSV]({{ "export/AstraDriver_cpl_jlc.csv" | absolute_url | append: cacheBust }})

#### Eurocircuits

- [Eurocircuits Zip]({{ "export/AstraDriver-Eurocircuits.zip" | absolute_url | append: cacheBust }})
- [Eurocircuits BOM CSV]({{ "export/AstraDriver_bom_Eurocircuits.csv" | absolute_url | append: cacheBust }})
- [Eurocircuits CPL CSV]({{ "export/AstraDriver_cpl_Eurocircuits.csv" | absolute_url | append: cacheBust }})

#### 3D Step

- [3D Step]({{ "/AstraDriver-3D.step" | absolute_url | append: cacheBust }})
  
## Report

#### ERC

{% include_relative erc_validation.md %}

#### DRC

{% include_relative drc_validation.md %}

{% include_relative AstraDriver-report.md %}

## Know Issues

- TBD

## Credits

[KiCad EDA](https://www.kicad.org)

[KiBot](https://github.com/INTI-CMNB/KiBot)

[Amulet - Inspiration for awesome schematic and PCB](https://github.com/EPFLXplore/XRE_LeggedRobot_HW)

[tracespace view - Online Gerber Viewer](https://tracespace.io)