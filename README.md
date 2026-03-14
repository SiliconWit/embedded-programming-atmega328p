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

A bare-metal C programming course for the AVR ATmega328P microcontroller. Lessons progress from toolchain setup and GPIO registers through communication protocols (UART, SPI, I2C), analog acquisition, and power management.

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

## File Structure

```
embedded-programming-atmega328p/
├── lesson-0.mdx        # Course introduction
├── lesson-1.mdx        # AVR Toolchain and Bare-Metal C
├── lesson-2.mdx        # GPIO Registers and Digital IO
├── lesson-3.mdx        # Timer Counter Fundamentals
├── lesson-4.mdx        # Interrupts and Event-Driven Design
├── lesson-5.mdx        # UART Serial Communication
├── lesson-6.mdx        # SPI and Peripheral Interfacing
├── lesson-7.mdx        # I2C Bus and Sensor Integration
├── lesson-8.mdx        # ADC and Analog Acquisition
├── lesson-9.mdx        # Power Management and Watchdog
└── README.md
```

## How to Contribute

1. Fork the repository: [SiliconWit/embedded-programming-atmega328p](https://github.com/SiliconWit/embedded-programming-atmega328p)
2. Create a feature branch: `git checkout -b feature/your-topic`
3. Make your changes and commit with a clear message
4. Push to your fork and open a Pull Request against `main`
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

Clone the main site repository and initialize submodules:

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
