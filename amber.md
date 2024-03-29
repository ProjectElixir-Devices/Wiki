![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Xiaomi 11T (agate/amber)

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
   - **Recovery Link [ For Android 14 ]:** [Project Elixir Recovery](https://sourceforge.net/projects/project-elixir/files/fourteen/amber/recovery/boot.img/download)

3. Download the Project Elixir ROM for Xiaomi 11T (agate/amber) from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/amber)

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
### Step 3: Flash Elixir Recovery using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the Elixir Recovery.

2. Download the TWRP Recovery img from the link provided in Step 1.

3. Place the downloaded Elixir Recovery image .img in the same location as the platform-tools folder on your computer.

4. Now, flash the Exilir Recovery using the following command:

```
fastboot flash boot recovery_file_name.img
```

**Replace `recovery_file_name.img` with the actual name of the Elixir Recovery image you downloaded if needed.**

5. After flashing the recovery, use the following command to reboot your Recovery:

```
fastboot reboot recovery
```

Your device will reboot with Elixir Recovery installed.

### Step 4: Wipe Data
1. Factory reset > Format data/factory reset

### Step 5: Flash Project Elixir ROM
1. Back to recovery home page & Apply update > Apply from ADB
2. Open command prompt & sideload rom using command 

```
adb sideload <rom_filename>.zip
```
3. After insatlling successfully reboot to system.

### Dirty Flashing Steps
1. Go to recovery
2. Apply update > Apply from ADB
3. Open command prompt & sideload rom using command

```
adb sideload <rom_filename>.zip
```

4. After finishing reboot and enjoy :D

> [!Note] 
> **Notes specific to device build**
> * Gapps are already included in zip no need to flash additionally
> * If you are coming from Android 12 or 13 to Android 14 then clean flash is compulsory and format data.

