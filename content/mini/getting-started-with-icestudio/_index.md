---
title: Getting Started with iCE Studio
type: docs
sidebar:
  open: true
weight: 2
next: /mini/getting-started-with-icestudio/what-is-icestudio/
---

New to FPGAs? You're in the right place! This section guides you through setting up **iCE Studio** and running your first visual hardware project on the **Soan Papdi Mini**—without writing a single line of code.

{{< callout type="info" >}}
**Why iCE Studio?** \
iCE Studio is an open-source visual editor for Lattice iCE40 FPGAs. Instead of writing complex HDL code from day one, you can build real digital circuits by dragging, dropping, and wiring logic blocks together—then upload them to your board with one click.
{{< /callout >}}

<br>

## What You'll Need

Before getting started, make sure you have:
- A **[Soan Papdi Mini ↗](https://www.ashoktinkeringlabs.com/soan-papdi-mini)** FPGA board.
- A **USB-C data cable** (make sure it supports data transfer, not just charging).
- A computer running **Windows, macOS, or Linux**.

<br>

## Step-by-Step Guide

Follow these steps in order to set up your environment and upload your first circuit:

{{% steps %}}

### Discover Your Visual Toolchain

Learn what **iCE Studio** is and how visual block-based design makes learning digital logic and FPGA hardware intuitive and fun.

{{< cards >}}
  {{< card link="/mini/getting-started-with-icestudio/what-is-icestudio/" title="What is iCE Studio?" icon="puzzle" subtitle="Explore visual block-based FPGA design" >}}
{{< /cards >}}

### Install iCE Studio

Download and set up iCE Studio on your operating system, install the built-in toolchain, and select the **Soan Papdi Mini** board.

{{< cards >}}
  {{< card link="/mini/getting-started-with-icestudio/installing-ice-studio/" title="Installing iCE Studio" icon="download" subtitle="Set up the IDE and board toolchain" >}}
{{< /cards >}}

### Build Your First Circuit

Create your first visual FPGA project from scratch by wiring up blocks to blink the onboard **Green RGB LED** on your Soan Papdi Mini.

{{< cards >}}
  {{< card link="/mini/getting-started-with-icestudio/blink-the-green-rgb-led/" title="Blink the Green RGB LED" icon="light-bulb" subtitle="Build and upload your first visual FPGA design" >}}
{{< /cards >}}

### Explore Built-in Examples

Ready to experiment further? Check out more built-in iCE Studio examples and see what else you can build.

{{< cards >}}
  {{< card link="/mini/getting-started-with-icestudio/explore-more-examples/" title="Explore More Examples" icon="sparkles" subtitle="Discover counters, sensors, and built-in circuits" >}}
{{< /cards >}}

{{% /steps %}}
