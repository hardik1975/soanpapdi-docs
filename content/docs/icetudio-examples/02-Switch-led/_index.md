---
title: 2. Switch & LED
type: docs
sidebar:
  open: false
weight: 2
Next: /docs/examples/03-blink-led/
---

<br>

<div style="text-align: center;">
  <video
    controls
    autoplay
    muted
    loop
    playsinline
    width="100%"
    style="border-radius: 12px; overflow: hidden;">
    <source src="/videos/examples/led-switch-example.mp4" type="video/mp4">
  </video>

  <p style="margin-top: 10px; font-size: 0.85rem; opacity: 0.65;">
    Controlling LED with Switch example.
  </p>
</div>

In this project, you'll turn on an onboard LED by using switch on the Soan Papdi board using Icestudio's visual logic blocks.

---

### What You Will Need

1. Soan Papdi FPGA Board ➜ [**Link**](https://www.ashoktinkeringlabs.com/soan-papdi)
2. USB Type-C data cable

---

{{% steps %}}

### Select the Board

  Ensure your target board is set to **Soan Papdi** in the bottom-right corner.

  ![Select the board](images/select-the-board.png)

  If you haven't set this up yet, see the detailed steps in [Example 1: Getting Started](../01-led/#select-the-board).

<br>

### Open the "Pushbutton & LED" Example

  Open the Pushbutton & LED example from the Icestudio examples menu:

  ![Open Switch & LED Example](images/switch-led-example.png)

  When you open this example, Icestudio will prompt you to convert the pin mappings for Soan Papdi:

  * Click on **`Convert`** to continue.

  ![pin-convertion](images/pin-convertion.png)

<br>


### Understand the Blocks

  ![Switch & LEDs](images/Switch-led-blocks.png)

  **How the Circuit Works?**

  * **`PUSHBUTTON`** (Input Block): Reads the switch position. Even though the block is named Pushbutton, it maps to the DIP slide switch on the Soan Papdi.

    <!-- 1. Slide ON ➜ sends high (1)
    2. Slide OFF ➜ sends low (0) -->
    
    1. Slide ON ➜ sends high (1)
    2. Slide OFF ➜ sends low (0)

  * **`Wire:`** Passes the signal straight from the switch to the LED.

  * **`LED`** (Output): Turns ON when it receives 1 and turns OFF when it receives 0.

  **Choose the LED pin:**

  We need to assign physical FPGA pins to both the input and output blocks.

  ![Pin Switch & LEDs](images/select-pin-switch-led.png)

  * LED Pin: Click the dropdown on the LED block and select D0.
  * Switch Pin: Click the dropdown on the PUSHBUTTON block and select the A0 pin.


<br>

### Build Your Project
  
  Click the Build button in the bottom-right corner to convert your visual blocks into an FPGA bitstream.

  ![Build example](images/build-example.png)

<br>

### Upload Your Project
    
  Your bitstream is ready. Now, let’s upload it to the **Soan Papdi**.


  #### Step A: Enter Programming Mode {class="no-step-marker"}
  
  Put your board into programming mode before flashing. If you haven't done this before, follow the steps in [Example 1: Getting Started](../01-led/#step-a-put-the-board-in-programming-mode).

  <br>
  
 <div style="text-align: center;">
  <video
    controls
    autoplay
    muted
    loop
    playsinline
    width="100%"
    style="border-radius: 12px; overflow: hidden;">
    <source src="/videos/soan-papdi-programming video.mp4" type="video/mp4">
  </video>

  <p style="margin-top: 10px; font-size: 0.85rem; opacity: 0.65;">
    Soan Papdi in programming mode - blinking white LEDs on S0, S1, and S2.
  </p>
</div>

  > If your project ever fails to upload, always check if you remembered to put the board in programming mode first!

  Now, let's send our project to the board.

  #### Step B: Upload the Bitstream  {class="no-step-marker"}

  1. Click the **Upload** icon in the bottom-right corner of iCEstudio.
    
  ![upload-bitstream](images/upload-bitstream.png)

  2. Once the upload is complete, press the **RESET** button on the board to start running your new design.

  <br>    

  <div style="text-align: center;">
  <video
    controls
    autoplay
    muted
    loop
    playsinline
    width="100%"
    style="border-radius: 12px; overflow: hidden;">
    <source src="/videos/examples/led-switch-example.mp4" type="video/mp4">
  </video>

  <p style="margin-top: 10px; font-size: 0.85rem; opacity: 0.65;">
    Controlling LED with Switch example.
  </p>
</div>



{{% /steps %}}