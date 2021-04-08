# RUN_REPORT
intro


## Table of Contents

- [Prerequisites](#prerequisites)
- [Hardware Support](#hardware-support)
- [Building](#building)
- [Using QEMU](#using-qemu)
- [Using BOCHS](#using-bochs)
- [Using Gem5](#using-gem5)
- [Rapid Development](#rapid-development)
- [Resources](#resources)
- [Maintainers](#maintainers)
- [License](#license)
- [Acknowledgements](#acknowledgements)


## Prerequisites

- `gcc` cross compiler or `clang` (experimental) 
- `grub` version >= ~2.02
- `xorriso` (for creating ISO images)
- `qemu` or `bochs` (for testing and debugging)

## Hardware Support

Nautilus works with the following hardware:

- x86_64 machines (AMD and Intel)
- Intel Xeon Phi, both KNC and KNL using [Philix](http://philix.halek.co) for easy booting
- As a Hybrid Virtual Machine (HVM) in the [Palacios VMM](http://v3vee.org/palacios)

Nautilus can also run as a virtual machine under QEMU, BOCHS, KVM, and in a simulated
environment using [Gem5](http://gem5.org/Main_Page)

## Building

First, configure Nautilus by running either
`make menuconfig` or `make defconfig`. The latter
generates a default configuration for you. The former 
allows you to customize your kernel build:

```Shell
$> ln -s /usr/bin/grub2-mkrescue /usr/bin/grub-mkrescue
```

