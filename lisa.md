![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Xiaomi 11 Lite NE 5G / Mi 11 LE (lisa)

### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Reboot to bootloader (fastboot)
- Connect your phone to PC
- fastboot flash dtbo dtbo.img
- fastboot flash vendor_boot vendor_boot.img
- fastboot flash boot boot.img
- fastboot reboot recovery
- Select Wipe data/factory reset & confirm
- Go back and select Apply update from ADB
- adb sideload Project-Elixir*.zip(or drag down the rom zip to cmd)

Then kindly perform a format data in the recovery afterwards.

Reboot! Enjoy! #Project-Elixir
```

### Dirty Flashing Steps
```
- Reboot to recover by holding power button and volume up simultaneously
- In the recovery menu select Apply update through ADB
- adb sideload Project-Elixir*.zip(or drag down the rom zip to cmd)
- After installation complete

Reboot! Enjoy! #KeepEvolving
```
### Notes:

- A14 recovery: [Tap here for link]()
- Rom comes with Gapps inbuilt.
- If you are coming from A12/A13 to A14 then clean flash must.
- Clean flash always recommended to get the best experience.
