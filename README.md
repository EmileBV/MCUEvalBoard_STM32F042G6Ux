# STM32F042G6Ux Evaluation Board

This project exists because I needed a way to experiment with a tiny, inexpensive, USB-enabled microcontroller. I like working with STM32 so there were two main options available: STM32F042 or STM32C071. I started another board with the latter but then found out the F042 was cheaper on LCSC.

I'm also trying out panelizing boards with this project to optimize the order prices, but mainly to learn for my next project this is leading up to.

## TODO List

- Redo the RGB LED footprint to match the physical part's pinout
  - The real part doesn't have the same pin numbers as the standard footprint in kicad libraries.
- Replace all 0201 ESD diodes with 0402 or larger versions
  - JLCPCB can't assemble 0201 on economical PCBA option.
- Figure out why all footprints have the wrong rotation.
- Enlarge USB-C port pads, they don't even extend past the part's pads right now, so it won't solder properly.
- Add screenshots of the board for this README
- Add cost estimates
- Add .ioc file for the pre-wired functionalities
    - USB
    - TIM with PWM channels for RGB
    - Clocks
