![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Redmi K20 Pro/Mi 9T Pro (raphael/in)

###  **Note:** 
- The device must have an unlocked bootloader. If you are moving from Android 9/10/11/12/13 to Android 14, it is necessary CLEAN FLASH (Format Data).

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [OFOX Recovery](https://nc.razrcloud.duckdns.org/s/rNGeDfT9CptrA35)

3. Download the Project Elixir ROM for Redmi K20 Pro/Mi 9T Pro aka Raphael from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/violet)

4. Download Firmware zip from link below:
   - **A11 FW Link**: [Tap Here for link](https://t.me/ElixerRaphael/7390)

5. Download legacy2retrofit zip from link below:
   - **Legacy2Retrofit Link**: [Tap Here for link](https://t.me/Al_Arabis_Cloud/108)

6. Download DFE Neo zip from link below
   - **DFE NEO Link**: [Tap Here for link](https://t.me/Al_Arabis_Cloud/298)

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

### Step 3: Flash OFOX Recovery using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

```
fastboot devices
```

If your device is listed, you are ready to flash the TWRP Recovery.

2. Download the OFOX Recovery ZIP (`.img` file will be in zip) from the link provided in Step 1.

3. Place the downloaded OFOX Recovery image (`.img` file) in the same location as the platform-tools folder on your computer.

4. Now, flash the OFOX Recovery using the following command:

```
fastboot flash recovery recovery_file_name.img
```

**Replace `recovery_file_name.img` with the actual name of the OFOX Recovery image you downloaded if needed.**

5. After flashing the recovery, use the following command to reboot your Recovery:

```
fastboot reboot recovery
```

Your device will reboot with OFOX Recovery installed.

### Step 4: Wipe Data
1. In OFOX Recovery, use the touch screen or physical buttons to navigate.

2. Select "Wipe" from the main menu.

3. Wipe Data and Davlik & cache and then proceed to format data by typing yes. And reboot to recovery again.

### Step 5: Clean Flash Encrypted (Recommended)
```
- Reboot to your current recovery 
- Wipe dalvik-cache-sytem-vendor-data 
- Flash latest ofox recovery by amir
- Flash legacy to retrofit dynamic by @raphael_alpha.zip
- Flash latest a11 firmware (If coming from miui)
- Flash Elixir rom
- Format Data (if your data on ext4 then change it to f2fs instead of format data)
- Reboot to system
- Enjoy
```

### Dirty Flashing Encrypted (if already using a14 elixir)
```
- Reboot to recovery
- Flash Elixir rom
- Reboot to system
- Enjoy
```

### Decrypted Flashing Step (Do at your own risk)

### Clean Flash Decrypted 
```
- Reboot to your current recovery 
- Wipe dalvik-cache-sytem-vendor-data 
- Flash latest ofox recovery by amir
- Flash legacy to retrofit dynamic by @raphael_alpha.zip
- Flash latest a11 firmware (If coming from miui)
- Flash Elixir rom
- Flash DFE Neo
- Reboot to system
- Enjoy
```

### Dirty Flashing (Decrypted)
```
- Reboot to recovery
- Flash Elixir rom
- Flash DFE Neo
- Reboot to system
- Enjoy
```

### Note:


- Gapps are already included in zip no need to flash additionally!
- ROM comes with retrofit dynamic partition and erofs system, and uses fbev2 (casefolding) encryption type.
- If you are coming from Miui rom/ports or Older AOSP roms = Format Data and flash latest firmware
- If you are coming from A12/A13 to A14 then clean flash is compulsory and format data.
- If you are encrypted do format Data before flashing build to avoid bugs.
- If you want to flash with decryption (DFE) then do that your own risk (your bug report will be ignored)
