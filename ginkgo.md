![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Redmi Note 8 / 8T (ginkgo / willow)

###  **Note:** 
- The device must have an unlocked bootloader. If you are moving from Android 9/10/11/12/13 to Android 14, it is necessary CLEAN FLASH (Format Data).

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [Project Elixir Recovery](https://www.pling.com/p/1738205/)

3. Download the Project Elixir ROM for Redmi Note 8 / 8T from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/ginkgo)

4. Download DFE zip from link below:
   - **DFE v4 Link**: [Tap Here for link](https://drive.google.com/file/d/1fxx11QOCxXJGvMDGC5lRnom-M0nf8Dhd/view?usp=sharing)

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

### Step 3: Flash Recovery using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the Recovery.

2. Download the Recovery ZIP (`.img` file will be in zip) from the link provided in Step 1.

3. Place the downloaded Recovery image (`.img` file) in the same location as the platform-tools folder on your computer.

4. Now, flash the Recovery using the following command:

```
fastboot flash recovery recovery_file_name.img
```

**Replace `recovery_file_name.img` with the actual name of the Recovery image you downloaded if needed.**

5. After flashing the recovery, use the following command to reboot your Recovery:

```
fastboot reboot recovery
```

Your device will reboot with Recovery installed.

### Step 4: Wipe Data & Flash Project Elixir ROM
1. In Recovery, use the touch screen or physical buttons to navigate.

2. Select "Factory Reset" from the main menu.

3. Format cache partition and then proceed to Format data/factory reset.

4. Go back to main menu -> goto "Apply update" -> goto "Apply from ADB".

5. Head over to your pc, Download the Project Elixir ROM from the link provided in Step 1.

6. Open CMD(Windows) or Terminal(Macos or Linux) in that location.

7. Now, flash the Project Elixir ROM using the following command(Make Sure your adb is installed & USB cable connected):

```
adb sideload ProjectElixir_4.0_ginkgo-XXXXX-OFFICIAL.zip
```
(Replace ProjectElixir_4.0_ginkgo-XXXXX-OFFICIAL.zip with the actual name of the Project Elixir ROM you downloaded.)

8. Flash DFE v4.zip for decryption (optional).

9. After insatlling successfully reboot to system.

### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Boot to Recovery - must use A14 recovery - link below
- Format Data & cache.
- Flash the latest build (dont flash fcrypt v3)
- Flash DFE v4.zip for decryption (optional)
- Reboot
```

### Dirty Flashing Steps

### Encryption to Encryption :
```
1. Download the Latest Build
2. Boot to A14 recovery
3. Flash ROM zip
4. Format Cache
5. Reboot
```

### DIRTY FLASH WHEN YOU ARE DECRYPTED [A14 to A14]
```
1. Download the Latest Build
2. Boot to A14 recovery
3. Format Cache.
3. Flash ROM zip
4. Flash Fcrypt DFE v4 [Compulsory]
5. Reboot
```

### Note:

- A14 recovery: [Tap here for link](https://www.pling.com/p/1738205/)
- DFE v4.zip : [Tap Here for link](https://drive.google.com/file/d/1fxx11QOCxXJGvMDGC5lRnom-M0nf8Dhd/view?usp=sharing)
- Gapps are already included in zip no need to flash additionally!
- If you are coming from ports & others = Format Data and flash latest firmware
- If you are coming from A12/A13 to A14 then clean flash is compulsory and format data.
- If you are encrypted do format Data before flashing build to avoid bugs.
