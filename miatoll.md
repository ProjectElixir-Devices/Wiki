![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Miatoll

###  **Note:** 
- The device must have an unlocked bootloader.
- If you are moving from Android 13 to Android 14, it is necessary to install stable MIUI firmware and perform a CLEAN FLASH (Format Data).

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the OrangeFox FBEv1 Recovery from the link below:
   - **Recovery Link [ For Android 12, 13, 14 ]:** [Recovery](https://www.pling.com/p/1628174/)

3. Download the stable MIUI firmware from the link below:
   - **Firmware Link**: [MIUI Firmware Updater](https://xiaomifirmwareupdater.com/firmware/)

4. Download the Project Elixir ROM for Miatoll from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/download)

5. (Optional) OTG + Pendrive. Save ROM, Firmware, and Recovery into the Pendrive.

### Step 2: Install ADB and Boot into Fastboot Mode
1. Make sure you have ADB (Android Debug Bridge) installed on your computer. If you haven't installed it yet, you can download the latest Android platform tools for Windows from the link provided in Step 1.

2. Extract the downloaded platform-tools zip file on your computer.

3. Connect your device to your computer using a USB cable.

4. Open a command prompt (Windows) or terminal (macOS and Linux) on your computer.

5. Navigate to the location where you extracted the platform-tools.

6. Enter the following command to check if your device is connected and detected by ADB:

```
adb devices
```

If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options.

8. Now, reboot your device into Fastboot Mode using the following command:

```
adb reboot bootloader
```

### Step 3: Flash Stable MIUI Firmware (fastboot)

### Step 4: Flash OrangeFox Recovery using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the OrangeFox Recovery.

2. Download the OrangeFox Recovery image (`.img` file) from the link provided in Step 1.

3. Place the downloaded OrangeFox Recovery image (`.img` file) in the same location as the platform-tools folder on your computer.

4. Now, flash the OrangeFox Recovery using the following command:

```
fastboot flash recovery recovery_file_name.img
```

**Replace `recovery_file_name.img` with the actual name of the OrangeFox Recovery image you downloaded.**

5. After flashing the recovery, use the following command to reboot your device:

```
fastboot reboot recovery
```

Your device will reboot with OrangeFox Recovery installed.

### Step 5: Flash Project Elixir ROM
1. Go back to the main menu in recovery.

2. Select "Install."

3. Navigate to the location where you downloaded the Project Elixir ROM.

4. Select the ROM file and swipe the slider to confirm the installation.

### Step 6: Wipe Data
1. In OrangeFox Recovery, use the touch screen or physical buttons to navigate.

2. Select "Wipe" from the main menu.

3. Tap on "Format Data" and confirm by typing "yes" (without quotes) to perform a factory reset. This will erase all data on your device.

### Step 7: Reboot
1. Once the ROM installation is complete, go back to the main menu in recovery.

2. Select "Reboot."

3. Congratulations! Your device should now boot into Project Elixir ROM.

### NOTE :
- First boot may take some time, so be patient. Once the device boots up, follow the on-screen setup instructions, and you should be ready to explore the new ROM.
- Remember, flashing custom ROMs carries some risks, and it may void your warranty. Make sure you understand the process and its consequences before proceeding.
- Enjoy your new Project Elixir ROM experience on Miatoll!
