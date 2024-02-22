![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Redmi K20 Pro/Mi 9T Pro (raphael/in)

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
   - **Recovery Link [ For Android 14 ]:** [OFOX Recovery](https://nc.razrcloud.duckdns.org/s/rNGeDfT9CptrA35)

3. Download the Project Elixir ROM for Redmi K20 Pro/Mi 9T Pro aka Raphael/Raphaelin from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/raphael)

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
> [!Important]
> If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options.

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
> [!Important]
> Replace `recovery_file_name.img` with the actual name of the OFOX Recovery image you downloaded if needed.

5. After flashing the recovery, use the following command to reboot your Recovery:

```
fastboot reboot recovery
```

Your device will reboot with OFOX Recovery installed.

### Step 4: Wipe Data
1. In OFOX Recovery, use the touch screen to navigate.

2. Select "Wipe" from the main menu.

3. Wipe Data and Davlik & cache and then proceed to format data by typing yes. And reboot to recovery again.

### Step 5: Flash Project Elixir ROM

**Retrofit Dynamic Partitions** `(v4.0 and above versions)` - Clean Flash
```
- Download the latest build (Need to clean flash if you are on 3.13 or below)
- Take a backup for safe side (If you are coming from 3.13 or below you need to do a clean flash)
- Flash provided recovery Retrofit Supported Recovery
- Boot to Retrofit Supported Recovery
- Wipe dalvik-cache-sytem-vendor-data (wipe only dalvik-cache-data if coming from other dynamic roms)
- Flash legacy to retrofit dynamic by @raphael_alpha.zip (skip if coming from other dynamic roms)
- Flash latest a11 firmware (If coming from miui or a10 fw based rom)
- Flash Elixir rom
- Flash DFE NEO (if you want to be decrypted or already decrypted)
- Format Data (if your data on ext4 then change it to f2fs instead of format data)
- Reboot to system
- Enjoy
```

**Retrofit Dynamic Partitions** `(v4.0 and above versions)` - Dirty Flash
```
- Boot to Retrofit Supported Recovery
- Wipe only Dalvik/cache
- Flash or sideload the ROM zip
﻿﻿- Note if you want to decryption or already decrypted then only flash DFE NEO
- Reboot System
```
> [!Warning]
> **NOTE: We have Switched Retrofit Dynamic Partitions from v4.0 or above**


**Legacy ROM** `(v3.13 or below versions)` - **Clean Flash**
```
1. Copy the Project Elixir ROM (v3.13 or below) file to Internal storage or use OTG
2. Boot In the recovery that supports Legacy ROM Android 13
3. Wipe dalvik-cache-system-vendor-data
4. Flash latest a11 firmware (If coming from miui or a10 fw based rom)
5. Go to Install and Navigate to the location where you have kept the Project Elixir ROM.
6. Select the ROM file and swipe the slider to confirm the installation.
7. If you want decryption then only Flash DFE (optional)
8. After insatlling successfully reboot to system.
```

**Legacy ROM** `(v3.13 or below versions)` - **Dirty Flash**

Encryption to Encryption :
```
1. Download the Latest Build
2. Boot to Android 13 recovery that support encryption
3. Flash ROM zip
4. Clear Dalvik and Cache in advance wipe
5. Reboot
```

Decryption to Decryption `(Android 13 to Android 13)`
```
1. Download the Latest Build
2. Boot to Android 13 recovery that support decryption
3. Clear Dalvik and Cache in advance wipe
3. Flash ROM zip
4. Flash DFE (Compulsory)
5. Reboot
```

> [!Important]
> **May Required Files:**
> * Retrofit Supported Recovery : [Tap Here for link](https://nc.razrcloud.duckdns.org/s/rNGeDfT9CptrA35)
> * Android 13 Legacy Recovery (For encrypted user's): [Tap here for link](https://t.me/Al_Arabis_Cloud/104)
> * Android 13 Legacy Recovery (For decrypted user's): [Tap here for link](https://t.me/Al_Arabis_Cloud/107)
> * Legacy2Retrofit.zip : [Tap Here for link](https://t.me/Al_Arabis_Cloud/108)
> * A11 Firmware.zip : [Tap Here for link](https://t.me/ElixerRaphael/7390)
> * DFE.zip (for a13) : [Tap Here for link](https://t.me/Al_Arabis_Cloud/299)
> * DFE NEO.zip (for a14) : [Tap Here for link](https://t.me/Al_Arabis_Cloud/298)


> [!Note] 
> **Notes specific to device build**
> * We have Switched Retrofit Dynamic Partitions from v4.0 or above
> * ROM comes with retrofit dynamic partition and erofs system, and uses fbev2 (casefolding) encryption type.
> * Gapps are already included in zip no need to flash additionally
> * If you are coming from Miui rom/ports or Older AOSP roms = Format Data and flash latest firmware
> * If you are coming from Android 12 or 13 to Android 14 then clean flash is compulsory and format data.
> * If you are encrypted do format Data before flashing build to avoid bugs.
> * If you want to flash with decryption (DFE NEO) then do that your own risk.
> * If you're facing storage permission issues in certain apps/games after clean flash, [Follow this](https://t.me/ElixerRaphael/8707)
