![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Redmi K40Pro/Pro+/Mi11i/Mi 11X Pro (haydn/haydnin)

###  **Note:** 
- The device must have an unlocked bootloader. If you are moving from Android 9/10/11/12/13 to Android 14, it is necessary CLEAN FLASH (Format Data).

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [TWRP Recovery](https://www.pling.com/p/1824941/)

3. Download the Project Elixir ROM for Redmi K40 Pro/Pro+/Mi 11i/Mi 11X Pro aka Haydn/Haydnin from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/RedmiK40Pro)

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

### Step 3: Flash TWRP Recovery using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the TWRP Recovery.

2. Download the TWRP.img (from the link provided in Step 1).

3. Place the downloaded TWRP.img in the same location as the platform-tools folder on your computer.

4. Now, flash the TWRP Recovery using the following command:

```
fastboot boot twrp.img
```

Your device will reboot with TWRP Recovery installed.

### Step 4: Flash Project Elixir 

### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Reboot to Recovery - must use A14 recovery - link below
- Wipe Data, Metadata, Cache & Dalvik-Cache
- Flash the latest build
- Reboot Recovery
- Format Data
- Reboot System
```

### Dirty Flashing Steps

```
- Reboot to recovery
- Flash the rom.zip
- Reboot to System
```

### Note:

- A14 recovery: [Tap here for link](https://www.pling.com/p/1824941/)
- Firmware and Gapps are already included in zip no need to flash additionally!
- If you are coming from A12/A13 to A14 then clean flash is compulsory and format data.

