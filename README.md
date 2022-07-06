# Sagetech MXS Driver for PX4-1.11.0-rc1

This repo contains a standalone driver for PX4 tag 1.11.0-rc1 for manaual injection into an existing PX4 source tree.

## Usage
Copy the `src/` folder into the `PX4-Autopilot` folder.

In the `default.cmake` for the specific board used, add the line `transponder/sagetech_mxs` under the `DRIVERS` section.

### Example:
`default.cmake` location for Pixhawk 2.4.8 board:
```
├── boards
│   └── px4
│       └── fmu-v3
│           └── default.cmake
```

Enable driver in the "DRIVERS" segction of the `default.cmake` file:
```
...
DRIVERS
    ...
    transponder/sagetech_mxs
MODULES
    ...
```
See the files in the `boards` directory of these repo for further examples.