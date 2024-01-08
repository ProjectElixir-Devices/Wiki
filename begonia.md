![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Redmi Note 8 Pro (begonia)

###  **Note:** 
- The device must have an unlocked bootloader. If you are moving from Android 9/10/11/12/13 to Android 14, it is necessary CLEAN FLASH (Format Data).

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [TWRP Recovery](https://www.pling.com/s/Phones/p/1790714)

3. Download the Project Elixir ROM for Redmi Note 8 Pro aka begonia from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/begonia)


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

2. Download the TWRP Recovery ZIP (`.img` file will be in zip) from the link provided in Step 1.

3. Place the downloaded TWRP Recovery image (`.img` file) in the same location as the platform-tools folder on your computer.

4. Now, flash the TWRP Recovery using the following command:

```
fastboot flash recovery recovery_file_name.img
```

**Replace `recovery_file_name.img` with the actual name of the TWRP Recovery image you downloaded if needed.**

5. After flashing the recovery, use the following command to reboot your Recovery:

```
fastboot reboot recovery
```

Your device will reboot with TWRP Recovery installed.

### Step 4: Wipe Data
1. In Recovery, use the touch screen or physical buttons to navigate.

2. Select "Wipe" from the main menu.

3. Wipe > Advanced Wipe > Cache, Dalvik, System, Data, Vendor.

### Step 5: Flash Project Elixir ROM
1. Then copy the Project Elixir ROM file to Internal storage or use OTG/SD card
2. In the main menu in recovery.
3. Select "Install."
4. Navigate to the location where you downloaded the Project Elixir ROM.
5. Select the ROM file and swipe the slider to confirm the installation.
6. Reboot to Recovery
7. Wipe > Format Data (Type Yes)
7. After insatlling successfully reboot to system.

### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Boot to Recovery - must use A14 recovery - link below
- Wipe > Advanced Wipe > Cache, Dalvik, System, Data, Vendor
- Flash the latest build 
- Reboot to Recovery
- Wipe > Format Data (Type Yes)
- Reboot
```

### Dirty Flashing Steps

```
1. Download the Latest Build
2. Boot to A14 recovery
3. Clear Dalvik and Cache in advance wipe
4. Flash ROM Zip
5. Reboot
```

### Note:

- A14 recovery: [Tap here for link](https://www.pling.com/s/Phones/p/1790714)
- Firmware and Gapps are already included in zip no need to flash additionally!
- If you are coming from ports or other roms = Format Data is mandatory
- If you are coming from A12/A13 to A14 then clean flash is compulsory and format data.
- If you are encrypted do format Data before flashing build to avoid bugs.
