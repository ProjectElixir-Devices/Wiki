![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Redmi Note 12 5G / POCO X5 5G (stone)

> [!Warning]
> * Your warranty is void. Or valid, probably?
> * Project Elixir is not responsible for any damage you made to your device. You have been warned!
> * We are not responsible for anything that may happen to your phone by installing custom ROMs.
> * We are not responsible for anything that may happen to your phone by installing any kernels.
> * You do it at your own risk and take the responsibility upon yourself
> * You are not to blame Project Elixir or its respected developers for any of your loss.
>
> **Basic Notes for all users:**  
> * The provided instructions are for Project Elixir based on Android 14.
> * These will only work if you follow every section and step precisely
> * Do not continue after something fails! Contact in support group for help
> * The device must have an unlocked bootloader & has Platform Tools installed in pc.
> * If you are moving from any other Android version to Android 14, it is necessary to do CLEAN FLASH (Format Data)
> * Take a backup for safe side (If you are coming from older Android version or doing a clean flash)
> * For any queries or help related to Elixir, join our support group : [Tap Here](https://telegram.me/Elixir_Discussion)

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link**: [Tap here to download](https://www.pling.com/p/2132476/)

3. Download the Project Elixir ROM for Redmi Note 12 5G / POCO X5 5G  from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/stone)

### Clean Flash
- Download the latest build
- Take a backup for safe side
- Download recovery
- Connect your phone to PC
- Reboot To Fastboot  (  Press  Both Power_button_key + Vol_down_key)

- Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the Elixir Recovery.

```
fastboot boot  twrp.img/elixir recovery
```
```
- After flashing the recovery, use the following command to reboot your Recovery:
```
fastboot reboot recovery
```
- Select Wipe Data/factory Reset & Confirm
- Go back and select Apply update from ADB
```
adb sideload Project-Elixir*.zip(or drag down the rom zip to cmd) & flash fw (if u want)
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

- A14 recovery and vendor: [Tap here for link](https://sourceforge.net/projects/project-elixir/files/fourteen/stone)
- Rom comes with Gapps inbuilt.
- Clean flash always recommended to get the best experience.
