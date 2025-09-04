
# For ClearCore users on Linux:

Until this fork gets merged and official support for the ClearCore is added (if at all) make sure that you add the following to the [Platformio udev rules](https://docs.platformio.org/en/stable/core/installation/udev-rules.html) to include the Clearcore's VID and PIDs:
```rules
ATTRS{idVendor}=="2890", ATTRS{idProduct}=="[80]022", MODE="0666", ENV{ID_MM_DEVICE_IGNORE}="1", ENV{ID_MM_PORT_IGNORE}="1"
```
This is for Linux users only to let all users access the device


# Atmel SAM: development platform for [PlatformIO](https://platformio.org)

[![Build Status](https://github.com/platformio/platform-atmelsam/workflows/Examples/badge.svg)](https://github.com/platformio/platform-atmelsam/actions)

Atmel | SMART offers Flash- based ARM products based on the ARM Cortex-M0+, Cortex-M3 and Cortex-M4 architectures, ranging from 8KB to 2MB of Flash including a rich peripheral and feature mix.

* [Home](https://registry.platformio.org/platforms/platformio/atmelsam) (home page in the PlatformIO Registry)
* [Documentation](https://docs.platformio.org/page/platforms/atmelsam.html) (advanced usage, packages, boards, frameworks, etc.)

# Usage

1. [Install PlatformIO](https://platformio.org)
2. Create PlatformIO project and configure a platform option in [platformio.ini](https://docs.platformio.org/page/projectconf.html) file:

## Stable version

```ini
[env:stable]
platform = atmelsam
board = ...
...
```

## Development version

```ini
[env:development]
platform = https://github.com/platformio/platform-atmelsam.git
board = ...
...
```

# Configuration

Please navigate to [documentation](https://docs.platformio.org/page/platforms/atmelsam.html).
