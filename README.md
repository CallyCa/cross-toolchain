# NodeOS cross toolchain

This package generate a cross-compiler based on [gcc](https://gcc.gnu.org/) and
[musl](musl-libc.org) ready to use on the NodeOS build system, but could be used
by other systems. You can be able to configure the target of the cross-compiler
by setting some optional build flags or environment variables:

- **-b**/**BITS**: select between 32 or 64 - only affects x86 builds
- **-c**/**CPU**: by default it will generate for the current CPU
- **-M**/**MACHINE**: target machine according QEmu definitions

This `bin` folder contain placeholders for `npm` during the install step. They
are being replaced later during the install process to their correct symlinks.
