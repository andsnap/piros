# piros

A Rust OS project

## Dependencies
Required tools to build the kernel.

```

rustup
qemu

```

## To Run
Commands to run the kernel in a qemu environment.

``` bash

rustup toolchain install nightly # to install the nightly toolchain for the bootloader crate
rustup default nightly # switching to the nightly toolchain
cargo build # building the binary
cargo bootimage # building the bootimage
qemu-system-x86_64 -drive format=raw,file=target/x86-piros/debug/bootimage-piros.bin # running the kernel in qemu

```
