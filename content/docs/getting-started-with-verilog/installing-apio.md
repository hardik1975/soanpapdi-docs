---
title: Installing Apio CLI
weight: 2
# next: /docs/verilog-example/servo-sweep/
next: /docs/verilog-example/servo-sweep/
---

Ready to get started? Let's get the Apio CLI installed and configured on your machine.

<br>

## Setup Guide

{{% steps %}}

### Install Apio

First, you'll need to install the Apio CLI. You can do this using `pip` (Python's package manager) or by downloading a standalone installer for your operating system.

Follow the official [**Apio CLI Installation Guide ↗**](https://fpgawars.github.io/apio/docs/installing-apio-cli/) to get it set up on your machine.

![Apio CLI documentation](../../images/verilog-workflow/apio-documentation.png)

### Verify Installation

Once you've installed it, let's make sure everything is working correctly. Open your terminal or command prompt and run:

```bash
apio --version
```

If the installation was successful, you should see a response with the version number, like `Apio CLI version 1.5.1`.

![Apio version](../../images/verilog-workflow/apio-version.png)

### Download Board Packages

Apio supports many different FPGA boards out of the box, but you need to tell it to fetch the necessary packages. In your terminal, run:

```bash
apio boards
```

Apio will automatically connect to the internet and download the latest board definitions.

![Fetch Apio boards](../../images/verilog-workflow/fetch-apio-boards.JPG)

### Check Supported Boards

After the download is complete, verify that our board is ready to go. You should now see **Soan Papdi** listed among the supported boards in your terminal output.

![Soan Papdi in boards](../../images/verilog-workflow/soan-papdii-board-manager.png)

That's it! Your Apio setup is complete and ready for action. 🥳

{{% /steps %}}

<!-------------------------------------------------------------------------->

<br>

## Anatomy of an Apio Project

Before we start coding, it's helpful to understand how an Apio project is structured. Every project typically requires three main files to work:

1. **`apio.ini`** : Tells Apio which board you are using.
2. **`pins.pcf`** : Maps the FPGA's physical pins to names you can use in your code.
3. **`your_design.v`** : Your actual Verilog code (e.g., `servo.v`).
