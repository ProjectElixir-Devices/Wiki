![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png)

### Installation Guide For Project Elixir on OnePlus 7 (guacamoleb)

### Clean Flash
```
- First unlock bootloader on OxygenOS 11
- Install OOS 12.1 version 11.H.40 or 11.H.41 (depending on the region)
- After installation, download the .zip file with the above update via Oxygen Updater
```
- Download and run [OP Local Update](https://oxygenos.oneplus.net/OPLocalUpdate_For_Android12.apk) 
- Run the installation a second time (the second slot will be flashed)
```
- adb reboot bootloader
- Download Recovery from Pixel Experience Plus 13.0
- Fastboot flash boot_a boot.img and fastboot flash boot_b boot.img
- Now boot into recovery
- Format Data on both slots**
- Flash Project Elixir zip in recovery via adb sideload
- Now Reboot.
```

** If you don't see the slot switch, go back to bootloader and set it active via fastboot set_active a or fastboot set_active b and go back to recovery)
- [Recovery link of Pixel Experience Plus](https://get.pixelexperience.org/changelog/guacamoleb/PixelExperience_Plus_guacamoleb-13.0-20230714-2238-OFFICIAL.img)
