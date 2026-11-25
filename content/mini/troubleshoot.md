---
title: Troubleshoot
type: docs
weight: 7
prev: /mini/getting-started-with-verilog/blink-red-rgb-led/
sidebar:
  open: true
---

Running into an issue while using your **Soan Papdi Mini**? Don’t worry—we’ve got you covered. Below are quick solutions to the most common issues you may encounter.

Can’t find a solution here? **We’re happy to help!** \
Call us at **+91 9026278822** or email us at [hardikseth1975@gmail.com](mailto:hardikseth1975@gmail.com).

<!-------------------------------------------------------------------------->

<br>

## 1. `"icestudio.app is damaged"` Error (macOS)

If you are on a Mac and see an alert saying **`"icestudio.app" is damaged and can't be opened`**:

![iCE Studio macOS error](/docs/images/Getting%20Started%20Doc/icestudio-is-damaged-cant-open.png)

### The Fix

Don't panic—your application isn't broken! macOS Gatekeeper blocks unsigned apps downloaded from the internet by default. To clear the quarantine flag, open **Terminal** and run:

```bash
xattr -c /Applications/icestudio.app
```

*(Note: If your macOS installation placed the app on the Data volume, run `xattr -c /System/Volumes/Data/Applications/icestudio.app`).*

Once you run that command, iCE Studio will launch normally:

![Opening iCE Studio](/mini/getting-started-with-icestudio/images/open-icestudio.png)

<!-------------------------------------------------------------------------->

<br>

## 2. Board Failing to Upload

If your upload fails in iCE Studio or `apio upload` reports `Error: No matching USB device`, your **Soan Papdi Mini** is most likely not in **Programming Mode**.

![Upload Error](/docs/images/Getting%20Started%20Doc/trouble%20shoot/upload-error.png)

### The Fix

Before uploading any new design to the FPGA, you must put the **Soan Papdi Mini** into **Programming Mode** so its DFU bootloader listens for a new bitstream.

{{< callout type="warning" >}}
**#1 Cause of Upload Failures:** \
Always make sure the onboard **RGB LED is blinking white** before clicking **Upload** in iCE Studio or running `apio upload`!
{{< /callout >}}

### How to Enter Programming Mode on Soan Papdi Mini

{{% steps %}}

#### Press and hold the PROG button
Keep the **PROG** button held down.

#### Press and release the RESET button
While still holding **PROG**, press and release the **RESET** button. The onboard **Blue RGB LED** will turn on.

#### Release the PROG button
Let go of the **PROG** button.

#### Confirm the blinking White RGB LED
The onboard **White RGB LED** will begin blinking. Your **Soan Papdi Mini** is now in **Programming Mode** and ready to receive your bitstream!

{{% /steps %}}

<br>

<div style="text-align: center;">
  <video
    controls
    autoplay
    muted
    loop
    playsinline
    width="100%"
    style="border-radius: 12px; overflow: hidden; box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);">
    <source src="/videos/soan-papdi-mini-programming.mp4" type="video/mp4">
  </video>

  <p style="margin-top: 10px; font-size: 0.85rem; opacity: 0.65;">
    Soan Papdi Mini entering Programming Mode — watch for the Blue LED followed by the blinking White RGB LED.
  </p>
</div>

Once the **White RGB LED** is blinking, click **Upload** in iCE Studio (or run `apio upload`). When the upload finishes, press the **RESET** button once to exit Programming Mode and run your new circuit!

<!-------------------------------------------------------------------------->

<br>

## 3. Board Still Not Detected Over USB?

If your **Soan Papdi Mini** is blinking white in Programming Mode but your computer still doesn't detect it:

1. **Check Your USB-C Cable (Data vs. Charge-Only)**:
   Many USB-C cables included with power banks or headphones only carry power wires (`5V` and `GND`) and lack `D+`/`D-` data lines. Try a known **USB-C data cable** and verify detection by running:
   ```bash
   apio devices scan-usb
   ```
2. **Check `board` in `apio.ini` (Verilog / Apio CLI Users)**:
   If `apio devices scan-usb` shows `Soan Papdi FPGA (DFU)` and `apio upload` fails with `FILTER [VID=1D50, PID=6146, REGEX="^Soan Papdi Mini.*"]`, set `board = soan-papdi` in your project's `apio.ini`:
   ```ini
   [env:default]
   board = soan-papdi
   top-module = blink
   ```
