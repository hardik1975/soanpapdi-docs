---
title: Getting Started with Verilog
type: docs
sidebar:
  open: true
weight: 4
next: /mini/getting-started-with-verilog/what-is-apio/
---

Ready to go beyond visual blocks and design hardware with code? In this section, we'll walk you through the complete **Verilog** workflow for the **Soan Papdi Mini** using the open-source **Apio CLI**.

{{< callout type="info" >}}
**Why Verilog + Apio?** \
Verilog lets you describe digital circuits at the hardware level with full control over timing, state machines, and peripherals. **Apio** handles the entire open-source iCE40 toolchain (Yosys, nextpnr, and programmer tools) behind the scenes—so you can build and flash your board in seconds from the terminal.
{{< /callout >}}

<br>

## What You'll Need

Before diving in, make sure you have:
- A **[Soan Papdi Mini board↗](https://www.ashoktinkeringlabs.com/soan-papdi-mini)** FPGA board.
- A **USB-C data cable** (make sure it supports data transfer, not just charging).
- A code editor (such as **VS Code**).

<br>

## Step-by-Step Guide

Follow these steps in order to set up your environment and run your Verilog design:

{{% steps %}}

### Meet Your Toolchain

Learn what **Apio** is, how it manages the open-source FPGA synthesis and place-and-route tools under the hood, and why it makes command-line FPGA development effortless.

{{< cards >}}
  {{< card link="/mini/getting-started-with-verilog/what-is-apio/" title="What is Apio?" icon="puzzle" subtitle="Explore the open-source Verilog toolchain" >}}
{{< /cards >}}

### Get Everything Installed

Install the Apio CLI on Windows, macOS, or Linux, fetch the board definitions, and verify that your **Soan Papdi Mini** is recognized and ready to program.

{{< cards >}}
  {{< card link="/mini/getting-started-with-verilog/installing-apio/" title="Installing Apio CLI" icon="download" subtitle="Set up Apio and board packages" >}}
{{< /cards >}}

### Build Your First Verilog Project

Time to write some hardware description code! Create a complete Apio project from scratch (`apio.ini`, `pins.pcf`, and Verilog source) to blink the onboard **Red RGB LED** on your Soan Papdi Mini.

{{< cards >}}
  {{< card link="/mini/getting-started-with-verilog/blink-red-rgb-led/" title="Blink the Red RGB LED" icon="light-bulb" subtitle="Write, synthesize, and upload your first Verilog design" >}}
{{< /cards >}}

{{% /steps %}}

<!-------------------------------------------------------------------------->

<!-- <br>

## Ready for More?

Once you've completed your first blink project, explore more hands-on hardware designs in our Verilog Examples section:

{{< cards >}}
  {{< card link="/mini/verilog-example/" title="Verilog Examples" icon="code" subtitle="Explore more projects for Soan Papdi Mini" >}}
{{< /cards >}} -->
