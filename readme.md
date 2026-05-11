# Lenovo TB710FU GSI Fixes
**Compatible Devices:** Lenovo Yoga Tab (2026), Xiaoxin Pad Pro GT, Lenovo TB710FU

This Magisk module is a comprehensive fix for the Lenovo TB710FU series when running Generic System Images (GSI). It addresses critical hardware-to-software translation issues that are often missing or broken in standard GSI builds.

## Features
* **Tablet UI Core:** Forces `ro.build.characteristics=tablet` to enable the taskbar and multi-pane layouts.
* **Boot Animation Rotation:** Fixes the sideways (90°) boot animation rendering issue.
* **Smart Cover Support:** Maps the proprietary `hall_irq` sensor (codes 252/253) to standard Sleep/Wake events.
* **Hardware Overlay (RRO):** Injects a optimized `config.xml` for accurate auto-brightness, 144Hz refresh rate support, and Wi-Fi hotspot fixes.

## Installation
1. Download the latest ZIP from the **Releases** tab.
2. Install via Magisk or KernelSU.
3. Reboot.

## Upstream Status
* [PR #85](https://github.com/TrebleDroid/device_phh_treble/pull/85) - rw-system.sh & keylayout (Pending)
* [PR #175](https://github.com/TrebleDroid/vendor_hardware_overlay/pull/175) - Framework Overlay (Pending)