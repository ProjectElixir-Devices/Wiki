![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Redmi Note 12 Pro Speed / POCO X5 Pro 5G (redwood)

###  **Note:** 
- The device must have an unlocked bootloader. If you are moving from Android 9/10/11/12/13 to Android 14, it is necessary CLEAN FLASH (Format Data).

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link**: [Tap here to download](https://www.pling.com/p/2118914/)

3. Download the Project Elixir ROM for Redmi Note 12 Pro Speed / POCO X5 Pro 5G  from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/redwood)

### Clean Flash
- Download the latest build
- Take a backup for safe side
- Download The Boot , Dtbo  And Vendor_boot Images  
- Connect your phone to PC
- Reboot To Fastboot  (  Press  Both Power_button_key + Vol_down_key)

- Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the Elixir Recovery.

```
fastboot flash dtbo dtbo.img
```
```
fastboot flash vendor_boot vendor_boot.img
```
```
fastboot flash boot boot.img
```
- After flashing the recovery, use the following command to reboot your Recovery:
```
fastboot reboot recovery
```
- Select Wipe Data/factory Reset & Confirm
- Go back and select Apply update from ADB
```
adb sideload Project-Elixir*.zip(or drag down the rom zip to cmd)
```
Then kindly perform a format data in the recovery afterwards.

Reboot! 

### Dirty Flashing Steps
```
- Reboot to recover by holding power button and volume up simultaneously
- In the recovery menu select Apply update through ADB
- adb sideload Project-Elixir*.zip(or drag down the rom zip to cmd)
- After installation complete

Reboot! Enjoy!
```
### Notes:

- A14 recovery and vendor: [Tap here for link](https://sourceforge.net/projects/project-elixir/files/fourteen/redwood)
- Rom comes with Gapps inbuilt.
- Clean flash always recommended to get the best experience.
