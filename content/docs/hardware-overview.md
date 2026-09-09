---
title: Hardware Overview
type: docs
weight: 1
next: /docs/getting-started-with-icestudio/
sidebar:
  open: true
---

The design is intentional - Just the FPGA, Flash memory, a USB-C port for power and loading circuits, and Basics Input/Output.

<br>

<!-------------------------------------------------------------------------->

## Pin Diagram

A quick roadmap of the board:

![Soan Papdi Pin Diagram](hardware-overview-media/images/soan-papdi-pin-diagram.png)

<br>

<!-------------------------------------------------------------------------->

## Tech Specs at a Glance

Here’s the technical rundown of what’s under the hood.

{{< callout type="info" >}}
**What is a LUT?** \
LUTs (Look-Up Tables) are the basic building blocks used to create digital circuits on an FPGA. With 5,280 of them, you have plenty of room for creative projects!
{{< /callout >}}

{{< cards >}}
  {{< card title="FPGA Core" subtitle="**Lattice iCE40UP5K**" >}}
  {{< card title="Logic Resources" subtitle="**5,280 LUTs**" >}}
  {{< card title="Embedded Memory" subtitle="120 Kb BRAM / 1 Mb SPRAM" >}}
  
  {{< card title="Internal Oscillators" subtitle="10 kHz and 48 MHz" >}}
  {{< card title="Hard IP" subtitle="2 × SPI, 2 × I²C" >}}
  {{< card title="DSP Resources" subtitle="8 × DSP Multiplier Blocks" >}}
  {{< card title="Onboard Storage" subtitle="128 Mbit SPI Flash" >}}
  {{< card title="Interface" subtitle="USB-C (DFU Bootloader)" >}}
  {{< card title="Power" subtitle="5 Volts" >}}
  {{< card title="Dimensions" subtitle="67.5mm x 45.5mm" >}}
  {{< card title="Platform" subtitle="Windows, macOS & Linux" >}}
  {{< card title="Toolchain" subtitle="iCE Studio • APIO • Yosys • IceStorm" >}}
  {{< card title="User Interface" subtitle="12 LEDs • 8 Switches • 10 GPIO" >}} 
{{< /cards >}}

<br>

## Board Tour

Let's take a closer look at the different parts of the board:

{{% steps %}}

### Output LEDs (D7–D0)

Along the top edge, you'll find **8 Output LEDs** (labeled D7 through D0). You can program these to light up and show the results of your circuits. 

*Note: These are **active high**, which means sending a "1" in your code turns them on.*

![Output LEDs](images/landing-page/soan-papdi-output-leds-marked.png)

### Status LEDs (S3–S0)

Right next to the main outputs are **4 White Status LEDs**. These are perfect for indicating the health or current state of your design. 

*Note: Unlike the main LEDs, these are **active low**, meaning sending a "0" turns them on.*

![Status LEDs](images/landing-page/soan-papdi-status-led-marked.png)

### Input Switches (A3–A0 & B3–B0)

At the bottom, we've included **8 Slide Switches** split into two groups (Set A and Set B). These are your primary way to manually send inputs (1s and 0s) directly into your FPGA designs.

![Input Switches](images/landing-page/soan-papdi-slide-switches-marked.png)

### GPIO Pins (IO0–IO9)

Want to connect external sensors, motors, or displays? The right side of the board features **10 General Purpose Input/Output (GPIO) pins**, allowing you to expand your projects far beyond the onboard hardware.

![GPIO Pins](images/landing-page/soan-papdi-gpio-marked.png)

{{% /steps %}}

<!-------------------------------------------------------------------------->

<br>

## Datasheet

For those who want to dive deep into the lowest-level details of the FPGA chip itself:

<br>

{{< pdf "hardware-overview-media/pdf/ice40-ultra-plus-data-sheet.pdf" >}}