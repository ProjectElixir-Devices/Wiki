![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

---

### Installation Guide For Project Elixir on OnePlus 7 Pro (guacamole)

---

### Clean Flash
- Download the latest build.
- Make sure you are using Oxygen OS 11 (v11.0.9.1). [Download Firmware](https://sourceforge.net/projects/evolutionx-guacamole/files/firmware_oneplus7pro.zip/download)
- Take a backup for safe side.
- Boot to TWRP for OOS 11. [Download TWRP](https://dl.twrp.me/guacamole/twrp-3.6.2_11-0-guacamole.img.html)
- Unlock Bootloader. Use: `fastboot oem unlock`
- Boot TWRP. Use: `fastboot boot twrp-3.6.2_11-0-guacamole.img`
- Wipe Dalvik/Cache + Data + Metadata.
- Reboot to TWRP.
- Flash the ROM.
- Reboot to system.

---

### Dirty Flashing Steps
**NOTE:** After you flash Elixir A14, TWRP is no longer supported.

- Reboot to Elixir Recovery.
- Sideload the new update.
- Reboot to system.

OR

- Perform a local update from the Updater.

---

### Notes:
- The ROM comes with GApps inbuilt.
- If you are coming from A12/A13 to A14, then a clean flash is a must.
- Clean flash is always recommended to get the best experience.
