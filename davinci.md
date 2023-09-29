![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For Project Elixir on Davinci

### Requirements:
- Latest global or chinese firmware from https://xiaomifirmwareupdater.com/firmware/davinci/ (if not already installed)
- Latest Dynamic FBEv2 TWRP from https://miracle.girlswithout.top/recoveries/TWRP/dynamic-fbev2/ (if not already installed)

- Kindly note that first move from normal partition to dynamic partition needs computer/laptop or otg to flash the rom

### Clean Installation instructions 
1. Flashing TWRP
- Run fastboot flash recovery twrp_davinci-xyz.img and fastboot reboot recovery to enter TWRP.

2. Updating firmware and flashing the ROM
- You must go to "Settings" in TWRP and disable "Unmount System before installing a ZIP" until you have installed a ROM.
- From TWRP, go to "Advanced" -> "ADB Sideload" and start a sideload. On your PC, run adb sideload fw_davinci_miui_DAVINCI_xyz.zip. When finished, start another sideload and run adb sideload ProjectElixir-x.xx-davinci-xyz.zip. Afterwards, head to "Wipe" -> "Format data" and confirm.
- You should re-enable "Unmount System before installing a ZIP" in the settings now if you disabled it earlier.

### Dirty Installation instructions
1. You must go to "Settings" in TWRP and disable "Unmount System before installing a ZIP" until you have installed a ROM
2. Flash the rom from internel storage or adb sideload
3. You should re-enable "Unmount System before installing a ZIP" in the settings now if you disabled it earlier
4. Restart the device