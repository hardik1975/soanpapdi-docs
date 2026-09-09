# Soan Papdi FPGA Documentation

Welcome to the official documentation repository for the **Soan Papdi** FPGA development board! 

This site is built using [Hugo](https://gohugo.io/) and the beautiful [Hextra](https://imfing.github.io/hextra/) theme. It serves as the central hub for all getting-started guides, visual programming tutorials (iCE Studio), Verilog examples, and hardware references.

## Getting Started Locally

Want to contribute to the documentation or run it locally on your machine? Follow these simple steps.

### Prerequisites

You will need to have **Hugo (Extended Version)** and **Git** installed on your system.
- [Install Hugo Extended](https://gohugo.io/installation/)
- [Install Git](https://git-scm.com/downloads)

### 1. Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/hardik1975/soan-papdi-docs.git
cd soan-papdi-docs
```

*(Note: Replace the URL with your actual repository URL if it differs!)*

### 2. Start the Development Server

Run the Hugo server to preview the site locally:

```bash
hugo server -D
```

Open your browser and navigate to `http://localhost:1313` to view the documentation. The site will automatically reload whenever you make changes to the markdown files!

## Contributing

We welcome contributions! Whether you're fixing a typo, adding a new Verilog example, or improving explanations, your help is appreciated.

All documentation content is written in Markdown and is located in the `content/` directory.

- The main documentation pages are inside `content/docs/`.
- Images and media are stored in `content/docs/images/`.

If you are adding new pages, remember to include the appropriate frontmatter at the top of your `.md` file so Hextra can format it correctly:
```yaml
---
title: Your Page Title
type: docs
weight: 10
---
```
