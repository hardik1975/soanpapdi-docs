---
title: Soan Papdi Mini Documentation
next: /mini/hardware-overview
weight: 1
cascade:
  type: docs
---

Welcome to the official **Soan Papdi Mini** documentation — a compact, breadboard-friendly **Lattice iCE40UP5K** FPGA development board built for hands-on learning, rapid prototyping, and digital logic design with an open-source FPGA toolchain.

<div class="board-showcase">

![Soan Papdi Mini FPGA](images/main-page/soan-papdi-mini-angled.png)

</div>

{{< callout emoji="⚡" >}}
**Compact size, full FPGA power:** \
Powered by the **Lattice iCE40UP5K** (`5,280 LUTs`), **27 breadboard-friendly GPIO pins**, an onboard **RGB LED**, **12 MHz oscillator**, and a **USB-C DFU bootloader**—programmable in seconds with 100% open-source tools on Windows, macOS, and Linux.
{{< /callout >}}

<div class="cta-row" style="display: flex; gap: 12px; flex-wrap: wrap; margin-top: 1.25rem; margin-bottom: 0.5rem;">
  <a href="/mini/hardware-overview/" style="display: inline-flex; align-items: center; gap: 8px; padding: 10px 20px; border-radius: 8px; text-decoration: none; font-weight: 600; background: var(--hextra-colors-background-secondary, #1f2937); color: var(--hextra-colors-text, #f9fafb); border: 1px solid var(--hextra-colors-border, #374151);">
    {{< icon "chip" >}} Explore Hardware & Pinout
  </a>
  <a href="https://www.ashoktinkeringlabs.com/soan-papdi-mini" target="_blank" rel="noreferrer" style="display: inline-flex; align-items: center; gap: 8px; padding: 10px 20px; border-radius: 8px; text-decoration: none; font-weight: 600; background: #3b82f6; color: white;">
    {{< icon "shopping-cart" >}} Get Soan Papdi Mini ↗
  </a>
</div>

<!-------------------------------------------------------------------------->

<br>

## Where Should I Start?

New to **Soan Papdi Mini**? Begin by exploring the board's pinout and hardware specs, then jump straight into your first visual circuit:

{{< cards cols="2" >}}
  {{< card link="/mini/hardware-overview/" title="Hardware Overview" subtitle="Explore the pinout diagram, 27 GPIOs, RGB LED channels, and iCE40UP5K specs." icon="chip" tag="Start Here" tagColor="info" >}}
  {{< card link="/mini/getting-started-with-icestudio/" title="Quickstart with iCE Studio" subtitle="Build and upload your first FPGA circuit visually in minutes—zero code required." icon="sparkles" tag="Beginner Friendly" tagColor="info" >}}
{{< /cards >}}

<!-------------------------------------------------------------------------->

<br>

## Choose Your Learning Path

You can program the **Soan Papdi Mini** visually using drag-and-drop logic blocks or directly in **Verilog HDL** from the command line. Pick the workflow that fits you best:

### 1. Visual Block Programming — iCE Studio

Ideal for beginners and visual learners. Wire up logic gates, counters, and clocks on a graphical canvas and flash your board with a single click.

{{< cards cols="2" >}}
  {{< card link="/mini/getting-started-with-icestudio/installing-ice-studio/" title="Install iCE Studio" subtitle="Download the pre-configured IDE for Windows, macOS, or Linux." icon="download" >}}
  {{< card link="/mini/getting-started-with-icestudio/blink-the-green-rgb-led/" title="Blink the Green RGB LED" subtitle="Build your first visual clock-divider circuit and flash it over USB-C." icon="light-bulb" tag="Tutorial" tagColor="info" >}}
{{< /cards >}}

### 2. Hardware Description Code — Verilog & Apio CLI

Ready to work closer to the silicon? Write synthesizable **Verilog** code and use the open-source **Apio CLI** (`Yosys` + `nextpnr`) to verify, build, and upload from your terminal.

{{< cards cols="2" >}}
  {{< card link="/mini/getting-started-with-verilog/" title="Getting Started with Verilog" subtitle="Learn the open-source Apio CLI workflow and project structure." icon="terminal" >}}
  {{< card link="/mini/getting-started-with-verilog/blink-red-rgb-led/" title="Blink the Red RGB LED" subtitle="Download and synthesize a complete Verilog counter design on Soan Papdi Mini." icon="code" tag="Project" tagColor="info" >}}
{{< /cards >}}

<!-------------------------------------------------------------------------->

<br>

## Resources & Support

Everything you need to download software packages, look up pinouts, and solve common setup issues:

{{< cards cols="2" >}}
  {{< card link="/mini/downloads/" title="Downloads" subtitle="Get iCE Studio installers, high-res pinout diagrams, starter projects, and datasheets." icon="download" >}}
  {{< card link="/mini/troubleshoot/" title="Troubleshooting" subtitle="Quick fixes for Programming Mode, macOS Gatekeeper alerts, and USB detection." icon="adjustments" >}}
{{< /cards >}}
