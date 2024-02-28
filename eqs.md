![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Moto Edge 30 Ultra/X30 Pro (eqs)

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

###  **Note:** 
- The device must have an unlocked bootloader. If you are moving from Android 12/13 to Android 14, it is necessary CLEAN FLASH (Format Data).
- Follow this guide to unlock bootloader :- [Click me](https://telegra.ph/Unlock-Bootloader-on-Moto-Edge-30-Ultra-11-25)

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [SHRP Recovery](https://projectelixiros.com/device/eqs)

3. Download the Project Elixir ROM for Moto Edge 30 Ultra/X30 Pro aka eqs from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/eqs)


### Step 2: Install ADB and Boot into Fastboot Mode
1. Make sure you have ADB (Android Debug Bridge) installed on your computer. 

2. Extract the downloaded platform-tools zip file on your computer.

3. Connect your device to your computer using a USB cable.

4. Open a command prompt (Windows) or terminal (macOS and Linux) on your computer.

5. Navigate to the location where you extracted the platform-tools.

6. Enter the following command to check if your device is connected and detected by ADB:

```
adb devices
```

If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options.

7. Now, reboot your device into Fastboot Mode using the following command:

```
adb reboot bootloader
```

### Step 3: Flash SHRP Recovery using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the SHRP Recovery.

2. Download the SHRP Recovery `.img` file from the link provided in Step 1.

3. Place the downloaded SHRP Recovery image (`.img` file) in the same location as the platform-tools folder on your computer.

4. Now, flash the SHRP Recovery using the following command:

```
fastboot flash recovery recovery_file_name.img
```

**Replace `recovery_file_name.img` with the actual name of the SHRP Recovery image you downloaded if needed.**

5. After flashing the recovery, use the following command to reboot your Recovery:

```
fastboot reboot recovery
```

Your device will reboot with SHRP Recovery installed.

### Step 4: Wipe Data
1. In SHRP Recovery, use the touch screen or physical buttons to navigate.

2. Select "Wipe" from the main menu.

3. Wipe Data and Davlik & cache and then proceed to format data by typing yes. And reboot to recovery again.

### Step 5: Flash Project Elixir ROM
1. Then copy the Project Elixir ROM file to Internal storage or use OTG/SD card
2. In the main menu in recovery.
3. Select "Install."
4. If you are coming from stock MyUI rom flash [THIS](https://mirrorbits.lineageos.org/tools/copy-partitions-20220613-signed.zip) in recovery first else device will bootloop.
5. Navigate to the location where you downloaded the Project Elixir ROM.
6. Select the ROM file and swipe the slider to confirm the installation.
7. After insatlling successfully reboot to system.

### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Boot to Recovery
- Format Data by typing yes
- Flash the latest build
- Reboot
```

### Dirty Flashing Steps

```
1. Download the Latest Build
2. Boot to recovery
3. Flash ROM zip
4. Clear Dalvik and Cache in advance wipe
5. Reboot
```

### Note:

- Gapps are already included in zip no need to flash additionally!
- If you are coming from A12/A13 to A14 then clean flash is compulsory and format data.
- Make sure you are on stock A12 firmware else device will bootloop!

<br>

> [!Important]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)
