---
title: Downloads
type: default
sidebar:
  hide: false
  exclude: true
toc: true
---

<p style="text-align: center; margin-top: -2.5rem; margin-bottom: 2.5rem; font-size: 1.125rem; color: var(--hextra-colors-text-muted, #9ca3af);">
  Everything you need for your <strong>Soan Papdi Mini</strong> — IDE installers, pinout diagrams, starter projects, and datasheets.
</p>

## iCE Studio Software

![iCE Studio](/mini/getting-started-with-icestudio/images/soan-papdi-icestudio-installation.png)

Download the pre-configured **Soan Papdi Mini** release of **iCE Studio** for your operating system:

{{< cards cols="3" >}}
  {{< card title="Windows (64-bit)" subtitle="Click to download installer" icon="download" tag=".exe" tagColor="info" link="https://github.com/hardik1975/soanpapdi-docs/releases/download/v1.0.0/windows-x64-SoanPapdiMini-icestudio.exe" >}}
  {{< card title="macOS" subtitle="Click to download disk image" icon="download" tag=".dmg" tagColor="info" link="https://github.com/hardik1975/soanpapdi-docs/releases/download/v1.0.0/macOS-SoanPapdiMini-icestudio.dmg" >}}
  {{< card title="Linux (x64)" subtitle="Click to download archive" icon="download" tag=".zip" tagColor="info" link="https://github.com/hardik1975/soanpapdi-docs/releases/download/v1.0.0/linux-x64-SoanPapdiMini-icestudio.zip" >}}
{{< /cards >}}

{{< callout type="info" >}}
**New to iCE Studio?** Follow our step-by-step **[Installing iCE Studio Guide](/mini/getting-started-with-icestudio/installing-ice-studio/)** to set up the IDE and built-in Apio toolchain.
{{< /callout >}}

<!-------------------------------------------------------------------------->

<br>
<br>

## Board Resources & Documentation

Helpful reference materials, starter projects, and hardware documentation for wiring and programming your **Soan Papdi Mini**.

<br>

### Pin Diagram

Keep this high-resolution pinout diagram handy to quickly map the 27 GPIO pins, power rails, 12 MHz clock (`Pin 35`), and onboard active-low RGB LED (`Pin 40`, `Pin 41`, `Pin 39`):

{{< cards cols="1" >}}
  {{< card title="Soan Papdi Mini Pin Diagram ↓" subtitle="High-resolution board pinout reference for GPIO, power, and RGB LED channels" icon="chip" tag="PNG" tagColor="info" link="/mini/images/hardware-overview/soan-papdi-mini-pin-diagram.png" >}}
{{< /cards >}}

<br>

### Starter Example Projects

Ready-to-run Verilog / Apio example projects pre-configured for the **Soan Papdi Mini**:

{{< cards cols="1" >}}
  {{< card title="Onboard Red RGB LED Blink (Verilog) ↓" subtitle="Complete Apio CLI project (apio.ini, pins.pcf, blink.v) ready to build and upload" icon="code" tag="ZIP" tagColor="info" link="/downloads/01-red-rgb-led-blink.zip" >}}
{{< /cards >}}

<br>

<!-- ### Fritzing Model

Use this Fritzing model to make circuit diagrams for your projects:

{{< cards cols="1" >}}
  {{< card title="Fritzing Model (.fzpz) ↓" link="/downloads/Soan Papdi Fritzing Model.fzpz" >}}
{{< /cards >}} -->

<br>

### Lattice iCE40UP5K Datasheet

Dive into the official silicon specifications, architecture, and electrical characteristics of the onboard **Lattice iCE40UP5K** FPGA:

{{< cards cols="1" >}}
  {{< card title="Lattice iCE40 UltraPlus Family Datasheet ↓" subtitle="Official technical datasheet covering LUT architecture, BRAM/SPRAM, PLL, and hard IP blocks" icon="document-text" tag="PDF" tagColor="warning" link="/downloads/iCE40-UltraPlus-Data-Sheet.pdf" >}}
{{< /cards >}}

<br>