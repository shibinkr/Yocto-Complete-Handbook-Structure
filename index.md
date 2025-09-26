📑 Index
<details> <summary><b>1. Introduction to Yocto</b></summary>

1.1 What is the Yocto Project?

1.2 History and Evolution of Yocto

1.3 Why Use Yocto Instead of Ubuntu/Debian?

1.4 Real-World Applications (IoT, Automotive, Networking, Aerospace)

</details> <details> <summary><b>2. Yocto Basics</b></summary>

2.1 Yocto, Poky, BitBake, and OpenEmbedded: What’s the Difference?

2.2 Understanding Layers, Recipes, and Metadata

2.3 Image Types (core-image-minimal, core-image-sato, custom)

2.4 The Role of Cross-Compilation

</details> <details> <summary><b>3. Getting Started</b></summary>

3.1 System Requirements and Host Setup

3.2 Installing Prerequisites (Ubuntu, Fedora, etc.)

3.3 Downloading Poky and Initial Setup

3.4 Building Your First Image

3.5 Exploring the Output Directory Structure

</details> <details> <summary><b>4. Anatomy of Yocto</b></summary>

4.1 What is a Recipe (.bb, .bbappend, .bbclass)?

4.2 Tasks and Variables (do_compile, do_install)

4.3 Layers (meta-*) and Their Purpose

4.4 Configuration Files (local.conf, bblayers.conf)

4.5 Package Groups and Images

</details> <details> <summary><b>5. Customization</b></summary>

5.1 Adding Extra Packages to an Image

5.2 Creating a Custom Layer (bitbake-layers create-layer)

5.3 Writing a New Recipe from Scratch

5.4 Modifying an Existing Recipe (.bbappend)

5.5 Kernel Customization (patches, configs, device tree)

</details> <details> <summary><b>6. Advanced Concepts</b></summary>

6.1 BitBake Workflow in Detail

6.2 Shared State Cache (sstate) and Reproducibility

6.3 Yocto Package Formats (ipk, rpm, deb)

6.4 SDK and Ext-SDK: Developing Outside the Build System

6.5 Multiconfig and Multilib Builds

6.6 License Compliance and Manifest Tracking

</details> <details> <summary><b>7. Debugging & Optimization</b></summary>

7.1 Common Yocto Build Errors and Fixes

7.2 Using bitbake -e and bitbake -c Commands

7.3 Debugging Recipe Dependencies

7.4 Reducing Image Size (strip, busybox, minimal images)

7.5 Performance Tuning and Build Acceleration (ccache, sstate mirror)

</details> <details> <summary><b>8. Target Deployment</b></summary>

8.1 Flashing Images to SD Cards, eMMC, NAND

8.2 Bootloader Basics (U-Boot)

8.3 Running Yocto Images in QEMU Emulator

8.4 Deploying to ARM, x86, MIPS, RISC-V Boards

8.5 Remote Debugging with gdbserver

</details> <details> <summary><b>9. Real-World Scenarios</b></summary>

9.1 Yocto for Raspberry Pi (meta-raspberrypi)

9.2 Building GUI with Qt (meta-qt5)

9.3 Adding Networking Tools and Services

9.4 Security Hardening in Yocto

9.5 Continuous Integration (Jenkins, GitLab CI, Buildbot)

</details> <details> <summary><b>10. Ecosystem and Tools</b></summary>

10.1 devtool: Fast Development and Testing

10.2 Toaster: Web UI for Yocto Builds

10.3 kas: Simplifying Multi-Layer Builds

10.4 Comparison with Other Build Systems (Buildroot, OpenWrt)

</details> <details> <summary><b>11. Resources & Community</b></summary>

11.1 Yocto Project Official Documentation

11.2 Commonly Used Layers (meta-openembedded, meta-virtualization)

11.3 Mailing Lists, IRC, and Forums

11.4 Books and Tutorials on Yocto

11.5 Commercial Support and Training Providers

</details>