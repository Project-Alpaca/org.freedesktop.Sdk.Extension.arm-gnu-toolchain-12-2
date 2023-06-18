# Arm GNU Toolchain Freedesktop SDK Extension

Downloads and repackages the official binary distribution of [Arm GNU Toolchain](https://developer.arm.com/Tools%20and%20Software/GNU%20Toolchain) as Flatpak.

## Why

To be able to do Arm embedded development (e.g. using Raspberry Pi Pico SDK) with Flatpak IDEs seamlessly without the need to resort to ugly hacks or modify the IDE package.

## Usage

- Use `flatpak-builder` to do the repackaging.
- Install the package.
- For your favorite IDE, add `arm-gnu-toolchain-12-2` to the `FLATPAK_ENABLE_SDK_EXT` environment variable via flatseal or  `flatpak override`.
- Restart the IDE and you should be able to invoke the toolchain without the need to mess with PATH or anything.
