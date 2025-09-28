# 11. Resources & Community

Yocto Project has a vibrant community and a wide array of resources to help developers, from official documentation to commercial training. This chapter highlights key resources for learning, troubleshooting, and extending Yocto.

---

## 11.1 Yocto Project Official Documentation

- The primary source of information for all aspects of Yocto.
- Includes user guides, reference manuals, and developer guides.
- Regularly updated with each Yocto release.

**Link:** [https://www.yoctoproject.org/docs](https://www.yoctoproject.org/docs)

---

## 11.2 Commonly Used Layers

- **meta-openembedded**: Provides extra recipes for applications, libraries, and utilities.  
- **meta-virtualization**: Contains recipes for virtualization tools like QEMU, KVM, and containers.  
- **meta-raspberrypi**: Hardware support and BSP for Raspberry Pi boards.  
- **meta-qt5**: Recipes for building Qt5 and GUI applications.  

**Example:** Adding a layer to your build:
   ```bash 
    bitbake-layers add-layer ../meta-openembedded/meta-oe
   ```

---

## 11.3 Mailing Lists, IRC, and Forums

- **Mailing Lists:** `yocto@lists.yoctoproject.org` for announcements and `yocto@lists.yoctoproject.org` for technical discussions.  
- **IRC:** `#yocto` on libera.chat for live help.  
- **Forums:** Community forums and Stack Overflow for Q&A.  


---

✅ **Summary**  
Yocto Project’s ecosystem is rich and active, with official documentation, widely used layers, community forums, and commercial support. Engaging with these resources accelerates learning, troubleshooting, and leveraging Yocto for embedded Linux projects.
