# 9. Real-World Scenarios

This chapter explores practical applications of Yocto in real-world embedded projects, showing how to leverage layers, packages, and tools effectively.

---

## 9.1 Yocto for Raspberry Pi (meta-raspberrypi)

- Use the `meta-raspberrypi` layer to build images tailored for Raspberry Pi boards.
- Supports Pi-specific bootloader, kernel, and device tree configurations.
- Example:
  ```bash
  TEMPLATECONF=meta-raspberrypi/conf source oe-init-build-env
  bitbake core-image-base
  ```
- Enables deploying minimal or full-featured images optimized for Raspberry Pi.

---

## 9.2 Building GUI with Qt (meta-qt5)

- Add the `meta-qt5` layer to include Qt libraries and tools.
- Build GUI applications that run natively on embedded Linux.
- Supports X11, Wayland, or framebuffer backends.
- Allows creating rich graphical interfaces for embedded devices.
- Example:
    ```bash
    bitbake qtbase
    bitbake qt5-image
    ```

---

## 9.3 Adding Networking Tools and Services

- Include packages such as `networkmanager`, `openssh`, or `iptables` via `IMAGE_INSTALL_append`. 
- Configure systemd services or init scripts for automated startup.
- Example in local.conf:
    ```bash
    IMAGE_INSTALL_append = " networkmanager openssh"
    ```
- Ensures networking capabilities and remote access in deployed images.

---

## 9.4 Security Hardening in Yocto

- Enable hardened toolchain and security features:
    - `EXTRA_OECONF += "--enable-stack-protector"`
    - Enable PIE, RELRO, and SSP for executables.

- Remove unnecessary services and packages to reduce the attack surface.
- Use Yocto features like `PACKAGECONFIG` to selectively build secure packages.

---

## 9.5 Continuous Integration (Jenkins, GitLab CI, Buildbot)

- Automate builds and tests using CI pipelines.
- Integrate Yocto build scripts into Jenkins or GitLab runners.
- Use shared `sstate caches` to accelerate CI builds.
- Example GitLab CI snippet:
    ```yaml
    build_image:
    script:
        - source oe-init-build-env
        - bitbake core-image-minimal
    ```

---

✅ **Summary**  
Real-world Yocto scenarios demonstrate how to deploy and customize images for Raspberry Pi, create GUIs with Qt, enable networking, implement security hardening, and integrate builds into CI pipelines. These practices accelerate embedded development and ensure production-ready Linux images.
