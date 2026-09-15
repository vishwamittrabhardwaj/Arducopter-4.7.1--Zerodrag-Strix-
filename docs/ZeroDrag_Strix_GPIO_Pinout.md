# ZeroDrag Strix FCU — UNOFFICIAL GPIO / Firmware Pinout

> ⚠️ **IMPORTANT: THIS IS NOT AN OFFICIAL ZERODRAG PINOUT.**
>
> This is a **community-derived GPIO and firmware function mapping** obtained through analysis of the ZeroDrag Strix FCU firmware. It is provided for reference, development, repair, and interoperability purposes.
>
> **Do not treat this document as an official ZeroDrag hardware specification.**

---

## About This Pinout

This document identifies the STM32 GPIO assignments found in the ZeroDrag Strix FCU firmware and the functions associated with those GPIOs.

The table has three columns:

- **GPIO #** — GPIO number used in the firmware/hardware definition.
- **STM32 Pin** — STM32 MCU port and pin designation.
- **Function in Firmware** — Function assigned to that GPIO in the firmware.

### Important

The **GPIO # is NOT the physical pin number of the STM32 MCU package**.

For example:

```text
GPIO # 23
    ↓
STM32 PB7
    ↓
I²C1 SDA
```

This does **not** mean that physical STM32 package pin 23 is PB7.

Likewise, this table should **not** be interpreted as an FCU connector/header pinout.

---

## STM32 GPIO / Firmware Mapping

| GPIO # | STM32 Pin | Function in Firmware |
|---:|---|---|
| 0 | PA0 | PWM/S3 – Motor/servo output 3 |
| 1 | PA1 | PWM/S4 – Motor/servo output 4 |
| 2 | PA2 | PWM/S5 – Motor/servo output 5 |
| 3 | PA3 | PWM/S6 – Motor/servo output 6 |
| 4 | PA4 | Battery 2 voltage ADC |
| 5 | PA5 | SPI1 SCK – IMU1 |
| 6 | PA6 | SPI1 MISO – IMU1 |
| 7 | PA7 | Battery 2 current ADC |
| 8 | PA8 | LED/PWM13 |
| 9 | PA9 | UART1 TX |
| 10 | PA10 | UART1 RX |
| 11 | PA11 | USB D− |
| 12 | PA12 | USB D+ |
| 13 | PA13 | SWDIO |
| 14 | PA14 | SWCLK |
| 15 | PA15 | Buzzer |
| 16 | PB0 | PWM/S1 – Motor/servo output 1 |
| 17 | PB1 | PWM/S2 – Motor/servo output 2 |
| 18 | PB2 | Not assigned / GPIO available |
| 19 | PB3 | SPI3 SCK – optical flow |
| 20 | PB4 | SPI3 MISO – optical flow |
| 21 | PB5 | SPI3 MOSI – optical flow |
| 22 | PB6 | I²C1 SCL |
| 23 | PB7 | I²C1 SDA |
| 24 | PB8 | UART4 RX |
| 25 | PB9 | UART4 TX |
| 26 | PB10 | I²C2 SCL |
| 27 | PB11 | I²C2 SDA |
| 28 | PB12 | SPI2 CS – OSD |
| 29 | PB13 | SPI2 SCK – OSD |
| 30 | PB14 | SPI2 MISO – OSD |
| 31 | PB15 | SPI2 MOSI – OSD |
| 32 | PC0 | Battery voltage ADC |
| 33 | PC1 | Battery current ADC |
| 34 | PC2 | Not assigned |
| 35 | PC3 | Not assigned |
| 36 | PC4 | Airspeed/pressure ADC |
| 37 | PC5 | Analog RSSI ADC |
| 38 | PC6 | UART6 TX |
| 39 | PC7 | UART6 RX |
| 40 | PC8 | SDMMC D0 |
| 41 | PC9 | SDMMC D1 |
| 42 | PC10 | SDMMC D2 |
| 43 | PC11 | SDMMC D3 |
| 44 | PC12 | SDMMC CLK |
| 45 | PC13 | Not assigned |
| 46 | PC14 | Not assigned |
| 47 | PC15 | SPI1 CS – IMU1 |
| 48 | PD0 | CAN1 RX |
| 49 | PD1 | CAN1 TX |
| 50 | PD2 | SDMMC CMD |
| 51 | PD3 | CAN1 silent control |
| 52 | PD4 | SPI3 CS – optical flow |
| 53 | PD5 | UART2 TX |
| 54 | PD6 | UART2 RX |
| 55 | PD7 | SPI1 MOSI – IMU1 |
| 56 | PD8 | UART3 TX |
| 57 | PD9 | UART3 RX |
| 58 | PD10 | PINIO1 |
| 59 | PD11 | PINIO2 |
| 60 | PD12 | PWM/S7 – Motor/servo output 7 |
| 61 | PD13 | PWM/S8 – Motor/servo output 8 |
| 62 | PD14 | PWM/S9 – Motor/servo output 9 |
| 63 | PD15 | PWM/S10 – Motor/servo output 10 |
| 64 | PE0 | UART8 RX |
| 65 | PE1 | UART8 TX |
| 66 | PE2 | External CS2 |
| 67 | PE3 | LED |
| 68 | PE4 | LED |
| 69 | PE5 | PWM/S11 – Motor/servo output 11 |
| 70 | PE6 | PWM/S12 – Motor/servo output 12 |
| 71 | PE7 | UART7 RX |
| 72 | PE8 | UART7 TX |
| 73 | PE9 | Not assigned |
| 74 | PE10 | Not assigned |
| 75 | PE11 | SPI4 CS – IMU2 |
| 76 | PE12 | SPI4 SCK – IMU2 |
| 77 | PE13 | SPI4 MISO – IMU2 |
| 78 | PE14 | SPI4 MOSI – IMU2 |
| 79 | PE15 | Not assigned |
| 80 | PF0 | Not assigned |
| 81 | PF1 | Not assigned |
| 82 | PF2 | Not assigned |
| 83 | PF3 | Not assigned |
| 84 | PF4 | Not assigned |
| 85 | PF5 | Not assigned |
| 86 | PF6 | Not assigned |
| 87 | PF7 | Not assigned |
| 88 | PF8 | Not assigned |
| 89 | PF9 | Not assigned |
| 90 | PF10 | Not assigned |
| 91 | PF11 | Not assigned |
| 92 | PF12 | Not assigned |
| 93 | PF13 | Not assigned |
| 94 | PF14 | Not assigned |
| 95 | PF15 | Not assigned |
| 96 | PG0 | Not assigned |
| 97 | PG1 | Not assigned |
| 98 | PG2 | Not assigned |
| 99 | PG3 | Not assigned |
| 100 | PG4 | Not assigned |

---

## Quick Reference

### Motor / Servo Outputs

| Output | STM32 Pin | GPIO # |
|---|---|---:|
| S1 | PB0 | 16 |
| S2 | PB1 | 17 |
| S3 | PA0 | 0 |
| S4 | PA1 | 1 |
| S5 | PA2 | 2 |
| S6 | PA3 | 3 |
| S7 | PD12 | 60 |
| S8 | PD13 | 61 |
| S9 | PD14 | 62 |
| S10 | PD15 | 63 |
| S11 | PE5 | 69 |
| S12 | PE6 | 70 |

### UARTs

| UART | TX | RX |
|---|---|---|
| UART1 | PA9 | PA10 |
| UART2 | PD5 | PD6 |
| UART3 | PD8 | PD9 |
| UART4 | PB9 | PB8 |
| UART6 | PC6 | PC7 |
| UART7 | PE8 | PE7 |
| UART8 | PE1 | PE0 |

### I²C

| Bus | SCL | SDA |
|---|---|---|
| I²C1 | PB6 | PB7 |
| I²C2 | PB10 | PB11 |

### SPI

| Bus | CS | SCK | MISO | MOSI |
|---|---|---|---|---|
| SPI1 – IMU1 | PC15 | PA5 | PA6 | PD7 |
| SPI2 – OSD | PB12 | PB13 | PB14 | PB15 |
| SPI3 – Optical Flow | PD4 | PB3 | PB4 | PB5 |
| SPI4 – IMU2 | PE11 | PE12 | PE13 | PE14 |

### CAN

| Interface | Signal | STM32 Pin |
|---|---|---|
| CAN1 | RX | PD0 |
| CAN1 | TX | PD1 |
| CAN1 | Silent Control | PD3 |

### Other Interfaces

| Function | STM32 Pin |
|---|---|
| USB D− | PA11 |
| USB D+ | PA12 |
| SWDIO | PA13 |
| SWCLK | PA14 |
| Buzzer | PA15 |
| SDMMC D0 | PC8 |
| SDMMC D1 | PC9 |
| SDMMC D2 | PC10 |
| SDMMC D3 | PC11 |
| SDMMC CLK | PC12 |
| SDMMC CMD | PD2 |
| PINIO1 | PD10 |
| PINIO2 | PD11 |

---

## ADC Inputs

| Function | STM32 Pin | GPIO # |
|---|---|---:|
| Battery voltage | PC0 | 32 |
| Battery current | PC1 | 33 |
| Airspeed / pressure | PC4 | 36 |
| Analog RSSI | PC5 | 37 |
| Battery 2 voltage | PA4 | 4 |
| Battery 2 current | PA7 | 7 |

---

## Method / Status

The mappings in this document represent functions identified in the analyzed firmware.

Where a GPIO is listed as **Not assigned**, this means no specific peripheral/function assignment was identified for that GPIO in the analyzed firmware configuration. It does not necessarily mean that the physical pin is electrically unused on the FCU.

The mapping may also differ between firmware versions or hardware revisions.

For this reason, users should verify the relevant signal electrically before connecting external hardware.

---

## Disclaimer

**This document is NOT an official ZeroDrag document.**

It is an independently produced, community-derived reference based on firmware analysis and hardware investigation.

ZeroDrag and Strix are referenced solely to identify the hardware to which this information relates.

Use this information at your own risk. Always verify electrical connections, voltage levels, and signal functions before connecting external hardware to the FCU.

**Do not use this document as a substitute for an official hardware schematic or manufacturer documentation.**
