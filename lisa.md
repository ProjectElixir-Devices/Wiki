![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Xiaomi 11 Lite NE 5G / Mi 11 LE (lisa)

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
> * Make sure you are using **Oxygen OS 11 (v11.0.9.1)**

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link**: [Tap here to download](https://www.pling.com/p/2120336/)

3. Download the Project Elixir ROM for Xiaomi 11 Lite NE 5G / Mi 11 LE aka Lisa from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/lisa)

### Clean Flash
- Download the latest build
- Take a backup for safe side
- Reboot to bootloader (fastboot)
- Connect your phone to PC
- Now, in fastboot flash recovery using the following command
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
- Boot to recovery 
- Select Wipe data/factory reset & confirm
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

Reboot! Enjoy! #KeepEvolving
```
### Notes:

- A14 recovery and vendor: [Tap here for link](https://www.pling.com/p/2120336/)
- Rom comes with Gapps inbuilt.
- If you are coming from A12/A13 to A14 then clean flash must.
- Clean flash always recommended to get the best experience.

<br>

> [!Important]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)
