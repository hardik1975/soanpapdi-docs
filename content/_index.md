---
title: "Soan Papdi FPGA"
toc: false
---

<div align="center" style="margin-top: 2rem;">

<!-- ### A beginner-friendly FPGA development board designed for students, makers and engineers. -->

### A beginner-friendly FPGA dev board designed for learning.

<br>

<!-- <div style="display: flex; gap: 8px; justify-content: center; flex-wrap: wrap; margin: 16px 0;">
  <a href="https://www.latticesemi.com/Products/FPGAandCPLD/iCE40UltraPlus"><img src="https://img.shields.io/badge/FPGA-Lattice_iCE40UP5K-blue" alt="FPGA"></a>
  <a href="#open-source-toolchain"><img src="https://img.shields.io/badge/Toolchain-Open--Source-green" alt="Toolchain"></a>
  <a href="#"><img src="https://img.shields.io/badge/Interface-USB--C-orange" alt="USB-C"></a>
</div> -->

<div class="cta-row" style="display: flex; gap: 16px; justify-content: center; margin-top: 1.5rem;">
  <a href="/docs/hardware-overview" class="cta-btn secondary" style="display: inline-flex; align-items: center; gap: 8px; padding: 10px 24px; border-radius: 8px; text-decoration: none; font-weight: 600; background: var(--hextra-colors-background-secondary, #e5e7eb); color: var(--hextra-colors-text, #374151);">
    {{< icon "menu" >}} Details
  </a>
  <a href="https://www.crowdsupply.com/ashoktinkeringlabs/soan-papdi" class="cta-btn primary" style="display: inline-flex; align-items: center; gap: 8px; padding: 10px 24px; border-radius: 8px; text-decoration: none; font-weight: 600; background: #3b82f6; color: white;">
    {{< icon "shopping-cart" >}} Crowd Supply
  </a>
</div>

</div>

<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/4.0.0/model-viewer.min.js"></script>

<div style="display:flex; justify-content:center; margin: 4rem 0;">
  <model-viewer
    src="./models/soan-papdi.glb"
    camera-controls
    auto-rotate
    rotation-per-second="6deg"
    auto-rotate-delay="3"
    interaction-prompt="visible"
    camera-orbit="0deg 0deg 80%"
    shadow-intensity="1.5"
    shadow-softness="1"
    environment-image="neutral"
    exposure="1.1"
    style="width: 100%; max-width: 800px; height: 450px; border-radius: 16px; background-color: var(--hextra-colors-background-secondary, #111827); box-shadow: 0 20px 40px -10px rgba(0,0,0,0.5); border: 1px solid var(--hextra-colors-border, #374151); overflow: hidden;">
  </model-viewer>
</div>

<div style="max-width: 800px; margin: 0 auto;">

<!-- ------------------- -->
<!-- <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/4.0.0/model-viewer.min.js"></script>

<div style="display:flex; justify-content:center; margin: 3rem 0;">
  <model-viewer
    src="./models/soan-papdi.glb"
    camera-controls
    camera-orbit="0deg 75deg 80%"
    shadow-intensity="1"
    environment-image="neutral"
    exposure="1.0"
    style="width: 100%; max-width: 800px; height: 400px; border-radius: 12px; background-color: var(--hextra-colors-background-secondary, #f9fafb);">
  </model-viewer>
</div>

<div style="max-width: 800px; margin: 0 auto;"> -->
<!-- ------------------- -->

{{< carousel >}}
![Angled](../docs/images/landing-page/1-soan-papdi-fpga-angled.jpg)
![Top](../docs/images/landing-page/2-soan-papdi-fpga-top.jpg)
![Bottom](../docs/images/landing-page/3-soan-papdi-fpga-bottom.jpg)
{{< /carousel >}}

</div>

{{< callout emoji="💡" >}}
  **The design is intentional:** \
  Just the FPGA, Flash memory, a USB-C port for power and loading circuits, and basic Input/Output to keep you focused on learning.
{{< /callout >}}

<br>

## New to FPGAs?

Most FPGA boards are designed for experienced engineers. You spend hours hunting for components, wiring up circuits, and debugging setups before writing a single line of code. **Soan Papdi is different.**

{{< cards >}}
  {{< card title="The Problem" icon="x-circle" subtitle="Most FPGA boards assume you are already an expert and know what you're doing." >}}
  {{< card title="The Soan Papdi Way" icon="check-circle" subtitle="Built for beginners with everything included: LEDs, switches, GPIOs, and USB power." >}}
{{< /cards >}}

<div style="margin: 2rem 0;">
  {{< youtube p9qrO0cj7SM >}}
</div>

<br>

### No Complex HDL Needed

No complicated installation flow. No lame driver installation. Download the IDE, double-click, and get started! Program it using the open-source **iCEStudio IDE** or use RAW HDL.

![Alternate Led Blink](../docs/images/landing-page/soan-papdi-alternate-led-blink.gif "Alternate LEDs blink example in iCE Studio.")

{{< cards >}}
  {{< card link="docs/getting-started" title="Getting Started Guide" icon="arrow-right" >}}
{{< /cards >}}

<br>

## Why this design?

Soan Papdi is designed for learning — every component has a reason.

### ➜  Output LEDs (D7–D0)

On top, we have 8 output LEDs (D7 to D0). These aren't random. We chose 8 yellow LEDs because 8-bit data is fundamental to digital systems. When you build things like counters, shift registers, state machines, or simple processors, you can visualize the output directly on the LEDs in real-time.

![Output LEDs](../docs/images/landing-page/soan-papdi-output-leds-marked.png)
*![8-bit counter example](../docs/images/8-bit-couter-example.gif "8-bit counter example on output leds")*

### ➜  Status LEDs (S3–S0)

Right next to the output LEDs are 4 white LEDs for status signals. Use them for carry flags, overflow indicators, error signals, or any custom status output — so you can see exactly what's happening inside your circuit at a glance.

![Status LEDs](../docs/images/landing-page/soan-papdi-status-led-marked.png)

### ➜  Input Switches (A3–A0 & B3–B0)

At the bottom side of the board, we have two sets of switches (Set A and Set B). These let you input two 4-bit values directly into your FPGA design. Build an adder, subtractor, comparator, or simple calculator, then change the inputs and observe the results instantly.

![Input Switches](../docs/images/landing-page/soan-papdi-slide-switches-marked.png)

### ➜  GPIO Pins (IO0–IO9)

On the right side of the board, 10 GPIO pins let you go beyond the onboard peripherals. Connect sensors, displays, motors, or your own custom hardware to extend the capabilities of Soan Papdi.

![GPIO Pins](../docs/images/landing-page/soan-papdi-gpio-marked.png)
*![IR sensor example](../docs/images/IR-sensor-example.gif "IR sensor example on GPIO pin")*

<br>

## Specification

<!-- | Feature | Description |
|---|---|
| **FPGA** | Lattice iCE40UP5K FPGA |
| **Logic Resources** | 5,280 LUTs (capable of hosting RISC-V soft-core CPUs) |
| **Memory** | 120 Kbit Block RAM + 1 Mbit (128 KB) Single-Port SPRAM |
| **Clocking** | On-chip PLL, Internal Oscillators: 10 kHz and 48 MHz |
| **Hard IP & DSP** | 2 × SPI, 2 × I²C, 8 × DSP multiplier blocks |
| **Storage** | 128 Mbit onboard SPI Flash |
| **User Interface** | 8× yellow LEDs, 4× white status LEDs, 8× DIP switches, 2× push buttons |
| **Expansion** | 10 × I/O pins for external sensors & peripherals |
| **USB & Power** | USB-C (5V), fully controlled by FPGA (no external MCU), DFU bootloader |
| **Toolchain** | iCE Studio, APIO, Yosys, nextpnr, IceStorm, Icarus Verilog, Amaranth HDL | -->

{{< cards >}}
  {{< card title="FPGA Core" subtitle="**Lattice iCE40UP5K**" >}}
  {{< card title="Logic Resources" subtitle="**5,280 LUTs**" >}}
  {{< card title="Embedded Memory" subtitle="**120 Kb BRAM / 1 Mb SPRAM**" >}}
  {{< card title="SPRAM" subtitle="**128 Mbit SPI Flash**" >}}
  {{< card title="Internal Oscillators" subtitle="**10 kHz and 48 MHz**" >}}
  {{< card title="Hard IP" subtitle="**2 × SPI, 2 × I²C**" >}}
  {{< card title="DSP Resources" subtitle="**8 × DSP multiplier blocks**" >}}
  {{< card title="Onboard Storage" subtitle="**128 Mbit onboard SPI Flash**" >}}
  {{< card title="Interface" subtitle="**USB-C (DFU Bootloader)**" >}}
  {{< card title="Power" subtitle="**5 Volts**" >}}
  {{< card title="Dimensions" subtitle="**67.5mm x 45.5mm**" >}}
  {{< card title="Platform" subtitle="**Windows, macOS & Linux**" >}}
  {{< card title="Toolchain" subtitle="**iCE Studio • APIO • Yosys • IceStorm**" >}}
  {{< card title="User Interface" subtitle="**12 LEDs • 8 Switches • 10 GPIO**" >}} 
{{< /cards >}}

<br>

## Learning Resources

To make things easier, **Piyush Itankar** has created a Digital Electronics 101 course, where everything is explained step-by-step.

{{< cards >}}
  {{< card link="https://www.youtube.com/playlist?list=PLTbERlX_4R03Ru_9ee6_U0GgTcg858amo" title="Soan Papdi FPGA 101 Course" icon="play" subtitle="Start learning on YouTube" >}}
{{< /cards >}}

Start simple — build basic gates like AND, OR, or a decoder. Once you're comfortable, move on to advanced projects:

1. **[RISC-V CPU](https://github.com/Obijuan/RISC-V-FPGA)** — A RISC-V processor implementation
2. **[Z80 CPU](https://github.com/Obijuan/Z80-FPGA)** — A recreation of the classic Z80 processor
3. **[Hack CPU](https://github.com/Obijuan/nand2tetris-icestudio)** — The Nand2Tetris Hack CPU, built gate by gate

<!-- ![Advanced FPGA projects](docs/images/landing-page/advanced-projects.png) -->

Looking for more inspiration? Browse the full **[iCEstudio Example Collection](https://github.com/FPGAwars/icestudio/wiki#organization-of-the-collection)**.

<br>

## The Team

Hardik & Lakshya created and built Soan Papdi from the ground up, turning an idea proposed by Piyush into a fully realized FPGA development board.

<div class="team-grid" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem; margin-top: 2rem;">

  <div class="member" style="background: var(--hextra-colors-background-secondary, #f3f4f6); padding: 2rem 1.5rem; border-radius: 12px; text-align: center; display: flex; flex-direction: column; align-items: center; border: 1px solid var(--hextra-colors-border, #e5e7eb); color: var(--hextra-colors-text, inherit);">
    <img src="docs/images/team/hardik1.jpg" style="width: 100px; height: 100px; border-radius: 50%; object-fit: cover; margin-bottom: 1rem; border: 3px solid var(--hextra-colors-border, #e5e7eb);">
    <h3 style="margin: 0; font-size: 1.25rem; color: var(--hextra-colors-text, #111827);">Hardik Seth</h3>
    <p style="margin: 0.25rem 0 1rem; font-size: 0.95rem; color: var(--hextra-colors-text-muted, #4b5563);"><strong>Embedded Engineer</strong><br>STEMpedia</p>
    <div style="display: flex; gap: 12px; justify-content: center; margin-bottom: 1rem; font-weight: 500; color: var(--hextra-colors-text-muted, #4b5563);">
      <a href="https://www.linkedin.com/in/hardik-seth-8687b7201/">LinkedIn</a> • 
      <a href="https://x.com/DIY_With_Hardik">X</a> • 
      <a href="https://www.youtube.com/@DIYwithHardik">YouTube</a>
    </div>
    <p style="font-size: 0.9em; text-align: left; line-height: 1.5; margin: 0; flex-grow: 1; color: var(--hextra-colors-text, #111827);">Engineer by day, Maker by night - playing with electronics since the age of 9. From childhood, I’ve loved tearing things apart, rebuilding them, and learning through hands-on experimentation. Currently working as an embedded engineer who designs PCBs, writes firmware, and enjoys turning ideas into complete, working hardware products.</p>
  </div>

  <div class="member" style="background: var(--hextra-colors-background-secondary, #f3f4f6); padding: 2rem 1.5rem; border-radius: 12px; text-align: center; display: flex; flex-direction: column; align-items: center; border: 1px solid var(--hextra-colors-border, #e5e7eb); color: var(--hextra-colors-text, inherit);">
    <img src="docs/images/team/piyush.jpg" style="width: 100px; height: 100px; border-radius: 50%; object-fit: cover; margin-bottom: 1rem; border: 3px solid var(--hextra-colors-border, #e5e7eb);">
    <h3 style="margin: 0; font-size: 1.25rem; color: var(--hextra-colors-text, #111827);">Piyush Itankar</h3>
    <p style="margin: 0.25rem 0 1rem; font-size: 0.95rem; color: var(--hextra-colors-text-muted, #4b5563);"><strong>Senior Embedded SW Engineer</strong><br>Google | Ex-Intel</p>
    <div style="display: flex; gap: 12px; justify-content: center; margin-bottom: 1rem; font-weight: 500; color: var(--hextra-colors-text-muted, #4b5563);">
      <a href="https://www.linkedin.com/in/streetdogg/">LinkedIn</a> • 
      <a href="https://x.com/_streetdogg">X</a> • 
      <a href="https://www.youtube.com/@pyjamacafe">YouTube</a>
    </div>
    <p style="font-size: 0.9em; text-align: left; line-height: 1.5; margin: 0; flex-grow: 1; color: var(--hextra-colors-text, #111827);">Electrical Engineer holding a Master’s degree in Embedded Systems, with a proven track record at industry giants. Currently thriving as an Embedded Software Engineer at Google, drove innovation in Firmware development for the Power Management Sub-system on Tensor SoCs and presently advancing system software for the Pixel Watch.</p>
  </div>

  <div class="member" style="background: var(--hextra-colors-background-secondary, #f3f4f6); padding: 2rem 1.5rem; border-radius: 12px; text-align: center; display: flex; flex-direction: column; align-items: center; border: 1px solid var(--hextra-colors-border, #e5e7eb); color: var(--hextra-colors-text, inherit);">
    <img src="docs/images/team/lsk.png" style="width: 100px; height: 100px; border-radius: 50%; object-fit: cover; margin-bottom: 1rem; border: 3px solid var(--hextra-colors-border, #e5e7eb);">
    <h3 style="margin: 0; font-size: 1.25rem; color: var(--hextra-colors-text, #111827);">Lakshya Seth</h3>
    <p style="margin: 0.25rem 0 1rem; font-size: 0.95rem; color: var(--hextra-colors-text-muted, #4b5563);"><strong>Digital Craftsman</strong><br>Class 12th Student</p>
    <div style="display: flex; gap: 12px; justify-content: center; margin-bottom: 1rem; font-weight: 500; color: var(--hextra-colors-text-muted, #4b5563);">
      <a href="https://www.linkedin.com/in/lakshyaseth7089/">LinkedIn</a> • 
      <a href="https://x.com/lakshya7089/">X</a> • 
      <a href="https://www.youtube.com/@lakshyaseth7089">YouTube</a>
    </div>
    <p style="font-size: 0.9em; text-align: left; line-height: 1.5; margin: 0; flex-grow: 1; color: var(--hextra-colors-text, #111827);">Love to build things, breaking and tearing things apart, to really learn how it's working, and what I can build with it. I like to play with Arch Linux and electronics. Currently, I'm in 12th grade and trying to get into an engineering college.</p>
  </div>

</div>

<br>

<div class="footer-note" style="text-align: center; margin-top: 3rem; margin-bottom: 2rem; font-size: 1.1em; color: var(--hextra-colors-text-muted, #6b7280);">
  Made with <span class="heart" style="color: #ef4444; font-size: 1.2em;">❤️</span> in India.
</div>