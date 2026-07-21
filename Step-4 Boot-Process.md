# Android Boot Process

The Android boot process begins in the device's Boot ROM and proceeds through the bootloader before loading the boot image (boot.img). The boot image contains the Linux kernel and the ramdisk. After the kernel initializes the hardware, it starts the Android init process, which launches system services and eventually the Android framework and user interface.

In this project, we are replacing only the kernel portion of the boot image while keeping the rest of the operating system intact.
