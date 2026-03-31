---
title: "Embedded Programming ATmega328P - Collaboration Guide"
description: "Contributing guide for Embedded Programming ATmega328P course content"
tableOfContents: true
sidebar:
  order: 999
---

# Embedded Programming ATmega328P

![Build](https://img.shields.io/badge/build-passing-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Contributors Welcome](https://img.shields.io/badge/contributors-welcome-orange)

**Read this course at:** [https://siliconwit.com/education/embedded-programming-atmega328p/](https://siliconwit.com/education/embedded-programming-atmega328p/)

A bare-metal C programming course for the AVR ATmega328P microcontroller. Lessons progress from toolchain setup and GPIO registers through communication protocols (UART, SPI, I2C), analog acquisition, power management, and integrated motor control.

## Lessons

| # | Title |
|---|-------|
| 1 | AVR Toolchain and Bare-Metal C |
| 2 | GPIO Registers and Digital IO |
| 3 | Timer Counter Fundamentals |
| 4 | Interrupts and Event-Driven Design |
| 5 | UART Serial Communication |
| 6 | SPI and Peripheral Interfacing |
| 7 | I2C Bus and Sensor Integration |
| 8 | ADC and Analog Acquisition |
| 9 | Power Management and Watchdog |
| 10 | Integrated Stepper Motion Control |

## File Structure

```
embedded-programming-atmega328p/
├── index.mdx
├── avr-toolchain-bare-metal-setup.mdx
├── gpio-registers-digital-io.mdx
├── timer-counter-fundamentals.mdx
├── interrupts-event-driven-design.mdx
├── uart-serial-communication.mdx
├── spi-protocol-peripheral-interfacing.mdx
├── i2c-bus-sensor-integration.mdx
├── adc-analog-signal-acquisition.mdx
├── power-management-watchdog-sleep.mdx
├── integrated-stepper-motion-control.mdx
└── README.md
```

## How to Contribute

All commands below work on Linux, macOS, and Windows (using Git Bash, PowerShell, or Command Prompt with Git installed).

### For Team Members (with push access)

**First time setup (clone the repo once):**

```bash
git clone https://github.com/SiliconWit/embedded-programming-atmega328p.git
cd embedded-programming-atmega328p
```

**Every time you start working:**

```bash
git pull origin main
```

Always pull before making changes. This avoids conflicts with other contributors.

**After making your changes:**

```bash
git add .
git commit -m "Brief description of what you changed"
git push origin main
```

**If you get a push error** (someone pushed before you):

```bash
git pull origin main
```

Git will merge the changes automatically in most cases. If there is a conflict, Git will mark the conflicting lines in the file. Open the file, choose which version to keep, then:

```bash
git add .
git commit -m "Resolve merge conflict"
git push origin main
```

**Tips to avoid conflicts:**

- Always `git pull origin main` before you start working
- Push your changes as soon as you are done, do not hold onto uncommitted work for long
- Coordinate with other contributors so two people are not editing the same file at the same time

### For External Contributors (without push access)

1. Fork the repository: [SiliconWit/embedded-programming-atmega328p](https://github.com/SiliconWit/embedded-programming-atmega328p)
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR-USERNAME/embedded-programming-atmega328p.git
   cd embedded-programming-atmega328p
   ```
3. Make your changes and commit:
   ```bash
   git add .
   git commit -m "Brief description of what you changed"
   git push origin main
   ```
4. Open a Pull Request against `main` on the original repository
5. Describe what you changed and why in the PR description

## Content Standards

- All lesson files use `.mdx` format
- Do not use `<BionicText>` in this course
- Code blocks should include a title attribute:
  ````mdx
  ```c title="blink.c"
  DDRB |= (1 << PB5);
  ```
  ````
- Use Starlight components (`<Tabs>`, `<TabItem>`, `<Steps>`, `<Card>`) where appropriate
- Keep paragraphs concise and focused on practical application
- Include working code examples that readers can compile and flash

## Local Development

To preview the full site locally, clone the main site repository and initialize submodules:

```bash
git clone --recurse-submodules <main-repo-url>
cd siliconwit-com
npm install
npm run dev
```

To test a production build:

```bash
npm run build
```

## License

This course content is released under the [MIT License](LICENSE).
