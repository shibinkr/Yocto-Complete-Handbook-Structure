# 8. Target Deployment

The Target Deployment chapter covers how to get Yocto-built images running on hardware or emulated environments, and how to debug them remotely.

---

## 8.1 Flashing Images to SD Cards, eMMC, NAND

- Use tools like `dd` or `bmaptool` to write images to SD cards.
- For eMMC or NAND storage, use board-specific flashing utilities or scripts.
- Ensure correct partition layout and bootloader installation for successful boot.

---

## 8.2 Bootloader Basics (U-Boot)

- U-Boot is the most common bootloader for embedded systems.
- Handles initialization of memory, peripherals, and loads the Linux kernel.
- Key steps:
  - Setting environment variables (bootargs, bootcmd)
  - Loading kernel and device tree blobs
  - Booting the root filesystem

---

## 8.3 Running Yocto Images in QEMU Emulator

- QEMU allows running Yocto images without physical hardware.
- Typical workflow:
  - Build a QEMU-compatible image (`core-image-minimal` or custom image)
  - Launch with `runqemu` or `qemu-system-ARCH` commands
  - Debug and test applications in a safe environment

---

## 8.4 Deploying to ARM, x86, MIPS, RISC-V Boards

- Cross-compiled images can be deployed to multiple architectures.
- Adjust MACHINE settings in `local.conf` for target hardware.
- Copy kernel, bootloader, and root filesystem to the device using `scp`, TFTP, or flashing tools.
- Verify board-specific drivers and device tree configurations.

---

## 8.5 Remote Debugging with gdbserver

- Use `gdbserver` on the target device to debug applications remotely.
- Steps:
  - Start `gdbserver` on target: `gdbserver :1234 ./my_app`
  - Connect from host using GDB: `target remote <IP>:1234`
  - Inspect variables, step through code, and monitor execution without stopping other processes.

---

✅ **Summary**  
Target Deployment covers all steps to get Yocto-built images running on physical boards or emulators, including flashing, bootloader setup, cross-platform deployment, and remote debugging. This ensures that development and testing can proceed efficiently on the intended hardware or simulation environment.
