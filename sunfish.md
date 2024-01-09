![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Google Pixel 4a (sunfish)

###  **Note:** 
- The device must have an unlocked bootloader. If you are moving from Android 12/13 to Android 14, it is necessary CLEAN FLASH (Factory reset).

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the boot image from the link below:
   - **Boot Image Link [ For Android 14 ]:** [Boot Image](https://www.pling.com/p/1980617/)

3. Download the Project Elixir ROM for Google Pixel 4a aka sunfish from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/sunfish)

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

### Step 3: Flash the boot.img using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the boot image.

2. Download the boot.img (from the link provided in Step 1).

3. Place the downloaded boot.img in the same location as the platform-tools folder on your computer.

4. Now, flash the boot image using the following command:

```
fastboot flash boot boot.img
```

Your device will reboot with TWRP Recovery installed.

### Step 4: Flash Project Elixir 

### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Boot into the recovery using the boot.img provided
- Do a factory reset after you entered into the recovery
- Flash the ProjectElixir.zip file through adb sideload
- Reboot System
```

### Dirty Flashing Steps

```
- Reboot to recovery
- Flash Rom zip file through adb sideload
- Reboot to System
```

### Note:

- A14 boot image: [Tap here for link](https://www.pling.com/p/1980617/)
- Gapps are already included in zip no need to flash additionally!
- If you are coming from A12/A13 to A14 then clean flash is compulsory and format data.
