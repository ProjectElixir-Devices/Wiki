![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Oneplus 6T (fajita)

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
> * If you are moving from any other Android version to Android 14, it is necessary to install stable OOS firmware and do CLEAN FLASH (Format Data)
> * Take a backup for safe side (If you are coming from older Android version or doing a clean flash)
> * For any queries or help related to Elixir, join our support group : [Tap Here](https://telegram.me/Elixir_Discussion)

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download Elixir Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [DOWNLOAD](https://www.pling.com/p/1866093/)

3. Download the stable OOS firmware from the link below:
   - **Firmware Link**: [OOS Firmware](https://download.h2os.com/OnePlus6T/MP/OnePlus6THydrogen_34.K.62_OTA_0620_all_2112282145_db7672c020714abb.zip)

4. Download the Project Elixir ROM for Fajita from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/download)

5. Download this super_empty.img file
   - **super_empty.img**: [DOWNLOAD](https://sourceforge.net/projects/project-elixir/files/fourteen/fajita/super_empty/)

6. Download this vbmeta.img file
   - **vbmeta.img**: [DOWNLOAD](https://sourceforge.net/projects/project-elixir/files/fourteen/fajita/vbmeta/)

### Step 2: Install ADB and boot to fastboot

> [!Important]
> **Note for Unlocking Bootloader**
> - Unlocking the bootloader will erase all data on your device! 
> - You cannot directly unlock the bootloader if you are on latest OxygenOS 12.1. For unlocked bootloader on OxygenOS 12.1, you will need to unlock the bootloader on OxygenOS 11 first and then update to OxygenOS 12.1
> - Before following these instructions please ensure that the device is currently using latest Android 12.1 firmware.

1. Make sure you have ADB (Android Debug Bridge) installed on your computer. 
2. Extract the downloaded platform-tools zip file on your computer.
3. Connect your device to your computer using a USB cable.
4. Open a command prompt (Windows) or terminal (macOS and Linux) on your computer.
5. Navigate to the location where you extracted the platform-tools.
6. Enter the following command to check if your device is connected and detected by ADB:
```
adb devices
```
> [!Important]
> - If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options
> - Enable OEM unlock in the Developer options under device Settings
> - You can also boot into fastboot mode via a key combination: turn the device off, hold `Volume Up + Volume Down + Power`

7. Now, reboot your device into Fastboot Mode using the following command:
```
adb reboot bootloader
```

### Step 3: Initializing Dynamic partitions
1. Download super_empty.img file
2. Boot it into bootloader mode if you are not in Fastboot mode
3. Flash vbmeta.img with the following commands:
```
fastboot flash vbmeta_a vbmeta.img
fastboot flash vbmeta_b vbmeta.img
```

### Step 4: Flash Recovery using Fastboot
4. Flash ProjectElixir Recovery:
```
fastboot flash boot boot.img
```
5. Erase the old android partitions with the following commands:
```
fastboot erase system_a
fastboot erase system_b
fastboot erase odm_a
fastboot erase odm_b
fastboot erase vendor_a
fastboot erase vendor_b
```
6. Now reboot into recovery and enter fastbootd mode
7. Initialize the retrofit super partitions for each slot:
```
fastboot wipe-super super_empty.img
fastboot set_active other
fastboot wipe-super super_empty.img
fastboot set_active other
```
8. Choose Enter recovery to return to recovery

### Step 5: Flash Project Elixir ROM from recovery
1. Download Project Elixir Rom Package.
2. If you are not in recovery, reboot into recovery [hold Volume Down + Power]
3. Now tap Factory Reset, then Format data / factory reset and continue with the formatting process. 
- This will remove encryption and delete all files stored in the internal storage, as well as format your cache partition (if you have one)
4. Return to the main menu.
5. Sideload the Project Elixir Rom.zip package:
6. On the device, select “Apply Update”, then “Apply from ADB” to begin sideload.
- On the host machine, sideload the package using:
```
adb sideload Rom.zip.
```
7. Once you have installed everything successfully, click the back arrow in the top left of the screen
8. Then “Reboot system now”.

> [!Note]
> - The first boot usually takes no longer than 15 minutes, depending on the device.
> - If the installation process reports the message "(~47%)
```
adb: failed to read the command: No error
```
> - Don't worry, the process was completed successfully and you can restart the device

<br>

> [!Important]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)
