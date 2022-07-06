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

Enable driver in the "DRIVERS" section of the `default.cmake` file:
```
...
DRIVERS
    ...
    transponder/sagetech_mxs
MODULES
    ...
```
See the files in the `boards` directory of this repo for further examples.

## More documentation
Further documentation on usage of the driver along with needed parameter config can be found here:

> [Sagetech MXS PX4 Support Driver](https://github.com/Sagetech-Avionics/Sagetech-Avionics.github.io/blob/main/documentation/PX4_MXS_PR.md)