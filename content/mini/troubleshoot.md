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

## 1. "icestudio.app is damaged" Error (macOS)

If you are on a Mac and see an alert saying:

 **`"icestudio.app" is damaged and can't be opened`**

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
**Cause of Upload Failures:** \
Always make sure the onboard **RGB LED is blinking white** before clicking **Upload** in iCE Studio or running `apio upload` .
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
    Soan Papdi Mini in Programming Mode.
  </p>
</div>

Once the **White RGB LED** is blinking, click **Upload** in iCE Studio (or run `apio upload` in your terminal).

{{< callout type="warning" >}}
**Don't Forget: Press the `RESET` Button After Uploading** \
After the upload finishes, your board stays in Programming Mode and won't run your project yet. **Press the RESET button once** on the board to exit Programming Mode and start running the code you just uploaded.
{{< /callout >}}

<!-------------------------------------------------------------------------->

<br>

## 3. Board Still Not Connecting to Your Computer?

If the **White RGB LED is blinking** (Programming Mode is active), but your project still won't upload, check these two things:

### Check 1: Use a Data USB-C Cable (Not a Charge-Only Cable)

Not all USB-C cables can transfer data! Many cheap cables included with power banks, wireless earbuds, or desk lamps are **charging-only**—they will light up the board, but your computer won't see the board at all.

**The Fix:**
- Switch to a **USB-C cable that supports data transfer** (such as a smartphone data cable).
- Try plugging the cable directly into a different USB port on your computer.

---

### Check 2: "No matching USB device" Error in Apio CLI (Verilog Users)

If you are uploading Verilog code from the terminal using `apio upload` and see this error:

```text
Error: No matching USB device.
```

**The Fix:** \
Open the `apio.ini` file in your project folder and make sure the board name is set to **`soan-papdi`**:

```ini
[env:default]
board = soan-papdi
top-module = blink
```

Save the file and run `apio upload` again—your code will upload right away!
