# Arducopter-4.7.1--Zerodrag-Strix
Ardupilot 4.7.1 firmware for Zerodrag Strix FCU
# ArduCopter 4.7.1 for ZeroDrag Strix FCU

This repository provides a **community-built ArduCopter 4.7.1 firmware upgrade for the ZeroDrag Strix Flight Controller Unit (FCU)**.

The firmware has been built and tested specifically for the **ZeroDrag Strix FCU** and is provided so that other users of the same hardware can upgrade their FCU without having to build the firmware themselves.

## Firmware Version

- **Flight Controller:** ZeroDrag Strix FCU
- **Firmware:** ArduCopter
- **Version:** 4.7.1
- **Target:** ZeroDrag Strix
- **Firmware files:** `.bin` and `.apj`

## Files

The repository contains the following firmware files:

| File | Description |
|---|---|
| `*.bin` | Binary firmware image |
| `*.apj` | ArduPilot firmware package |

The `.apj` file can be used with compatible ArduPilot firmware-loading tools, while the `.bin` file is provided as the raw firmware binary.

## Why this build?

The ZeroDrag Strix FCU did not have an readily available official 4.7.1 firmware release at the time this build was prepared.

This project provides a **4.7.1 build specifically prepared for the ZeroDrag Strix hardware**, allowing users to take advantage of the newer ArduPilot 4.7.1 firmware while continuing to use the Strix FCU.

## Installation

Before flashing:

1. **Make a complete backup of your current flight-controller parameters.**
2. Record your current firmware version.
3. Make sure you have a reliable USB connection to the FCU.
4. Disconnect unnecessary peripherals if appropriate.
5. Flash the supplied firmware using a compatible ArduPilot firmware-loading method.
6. After flashing, perform a full parameter check and re-calibration before flying.

### Using the `.apj` file

The `.apj` firmware file can be loaded using a compatible ArduPilot ground-control/firmware-loading tool.

Select the supplied `.apj` file and follow the normal firmware installation procedure.

### Using the `.bin` file

The `.bin` file is provided for users or tools that require the binary firmware image.

**Do not flash the firmware to hardware other than the intended ZeroDrag Strix target.**

## After Flashing

After the upgrade:

- Verify that the FCU boots normally.
- Confirm that the firmware reports **ArduCopter 4.7.1**.
- Check all sensor detection.
- Verify accelerometer and compass operation.
- Recalibrate sensors where required.
- Check radio input and output.
- Verify flight modes.
- Verify GPS and telemetry.
- Review all important parameters.
- Perform a thorough bench test before attempting flight.

A firmware upgrade can change parameters, defaults, or behaviour. **Do not assume that an aircraft configured on an older firmware version is immediately ready to fly after upgrading.**

## Important

This firmware is provided **as-is** for the ZeroDrag Strix FCU.

It is **not an official firmware release from ArduPilot or ZeroDrag**.

Although the firmware has been successfully flashed and tested on the intended hardware, users should understand that flashing custom firmware always carries some risk.

**Always maintain a backup of your working firmware and parameters before upgrading.**

The user is responsible for verifying the firmware, hardware configuration, parameters, and aircraft operation before flight.

## ArduPilot

This firmware is based on the open-source ArduPilot project.

ArduPilot:
https://github.com/ArduPilot/ardupilot

For information about ArduCopter 4.7.1, features, changes, and documentation, refer to the official ArduPilot project.

## Disclaimer

This repository is an independent community project.

The firmware is provided for users of the ZeroDrag Strix FCU who want to use ArduCopter 4.7.1.

**Use at your own risk.**

The author of this repository assumes no responsibility for damage to the flight controller, aircraft, equipment, property, or persons resulting from the use of this firmware.

## Credits

- **ArduPilot Project** — Open-source flight-control software
- **ZeroDrag** — Strix FCU hardware
- **Community contributors** — Firmware build, testing, and verification

---

### Firmware Status

**ArduCopter 4.7.1 — ZeroDrag Strix**

✅ Firmware built  
✅ `.bin` available  
✅ `.apj` available  
✅ Firmware flashed to ZeroDrag Strix FCU  
✅ Basic operation verified  

If you use this firmware successfully, consider sharing your results and configuration with the community.
