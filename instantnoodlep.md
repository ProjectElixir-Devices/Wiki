![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For Project Elixir on Instantnoodlep OOS11 (ver < 3.3)

1. Download Pixel/Los recovery and [ROM](https://www.pling.com/p/1813233/)
2. Reboot to bootloader
3. Flash recovery (guide [pixelexperience](https://wiki.pixelexperience.org/devices/instantnoodlep/install/))
4. Reboot to recovery
5. While in recovery, navigate to Apply update -> Apply from ADB
6. Install ROM
  ```
$ adb sideload rom.zip
  ```
6. Format data, reboot to system & Enjoy!

____

### Installation Guide For Project Elixir on Instantnoodlep OOS12 (ver >= 3.3)

1. Have an unlocked bootloader & OOS 12 (C20 - C33) [flashed to both slots](#guide-for-flashing-oos-12-in-both-slots)
2. Download Pixel/Los recovery and [ROM](https://www.pling.com/p/1813233/)
3. Reboot to bootloader
4. Flash recovery (guide [pixelexperience](https://wiki.pixelexperience.org/devices/instantnoodlep/install/))
5. Reboot to recovery
6. While in recovery, navigate to Apply update -> Apply from ADB
7. Install ROM
  ```
$ adb sideload ROM.zip
  ```
8. Format data, reboot to system & Enjoy!
____

#### Guide for flashing OOS 12 in both slots
(from any oos 11 custom rom)
1. Use [Msmtool](https://www.droidwin.com/unbrick-oneplus-8-pro-8t-msm-download-tool/#STEP_4_Download_MSM_Download_Tool_for_OnePlus_88_Pro) to come back on oos 11.
2. Download latest full zip of oos 12 from Oxygen Updater app or from OxygenOS builds [XDA thread](https://forum.xda-developers.com/t/oneplus-8-pro-rom-ota-oxygen-os-repo-of-oxygen-os-builds.4084315/) (You need to know your model number!)
3. Go into Settings -> system update -> local upgrade
4. Find the OOS 12 .zip you just downloaded from oxygen updater
5. Install it and reboot
6. Download and install the [OPLocalUpdate](https://forum.xda-developers.com/attachments/oplocalupdate_for_android12-apk.5747377/) apk
7. Repeat steps 4 to 6 (To install OOS 12 on both slots) using OPLocalUpdate
8. Unlock bootloader

Or [this guide](https://wiki.pixelexperience.org/devices/instantnoodlep/install/#ensuring-all-firmware-partitions-are-consistent).
