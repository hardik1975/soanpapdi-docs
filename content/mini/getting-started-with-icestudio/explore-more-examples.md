---
title: Explore More Examples
type: docs
weight: 4
prev: /mini/getting-started-with-icestudio/blink-the-green-rgb-led/
next: /mini/getting-started-with-verilog/
---

Now that you've blinked your first LED, you're ready to explore! **iCE Studio** includes a rich library of built-in examples that help you learn core FPGA concepts through hands-on experimentation.

<br>

## Accessing Built-in Examples

You can browse iCE Studio's built-in collection anytime from the top menu bar under **File → Examples**:

<br>

<video
  controls
  autoplay
  muted
  loop
  playsinline
  width="100%"
  style="border-radius: 12px; overflow: hidden;">
  <source src="/videos/icestudio-builtin-examples.mp4" type="video/mp4">
</video>

<!-------------------------------------------------------------------------->

<br>

## What You Can Build Next

With the **Soan Papdi Mini's** breadboard-friendly GPIO headers, you can wire up external LEDs, switches, and sensors to build complete digital systems:

### 1. Counters & Sequential Logic

A counter is one of the fundamental building blocks of digital electronics. By connecting external LEDs to the GPIO pins (or cycling through the **`R`**, **`G`**, and **`B`** channels), you can visualize binary counting and learn how **clocks**, **flip-flops**, and **registers** work together inside an FPGA.

<br>

<video
  controls
  autoplay
  muted
  loop
  playsinline
  width="100%"
  style="border-radius: 12px; overflow: hidden;">
  <source src="/videos/8-bit-counter.mp4" type="video/mp4">
</video>

<br>

### 2. Interfacing External Sensors (GPIO)

FPGAs excel at reading real-time hardware signals with zero software latency. You can connect an **IR proximity sensor**, push buttons, or other digital modules to a GPIO pin and route the signal through logic gates directly to an output LED or actuator.

<br>

<video
  controls
  autoplay
  muted
  loop
  playsinline
  width="100%"
  style="border-radius: 12px; overflow: hidden;">
  <source src="/videos/IR-sensor-example.mp4" type="video/mp4">
</video>

<!-------------------------------------------------------------------------->

<br>

## Keep Experimenting

These examples are just the starting point. The best way to master FPGA development is by tinkering:
- Combine multiple logic gates (**AND**, **OR**, **XOR**, **NOT**) to create custom combinational circuits.
- Drive multiple RGB channels (**`R`**, **`G`**, **`B`**) with different clock prescalers to create a color-cycling light show.
- Browse the community **[iCE Studio Collection Wiki ↗](https://github.com/FPGAwars/icestudio/wiki#organization-of-the-collection)** for even more blocks and examples.

<br>

{{< youtube I8ahqjVJAck >}}

<!-------------------------------------------------------------------------->

<br>

## Ready to Level Up to Verilog?

Once you're comfortable building circuits visually with blocks, take the next step and learn how to design hardware using **Verilog** and the **Apio CLI**:

{{< cards >}}
  {{< card link="/mini/getting-started-with-verilog/" title="Getting Started with Verilog" icon="terminal" subtitle="Learn how to write, synthesize, and upload Verilog code on Soan Papdi Mini" >}}
{{< /cards >}}
