<p align="center">
  <img src="https://github.com/Project-Elixir/docs/blob/bkl/res/elixir-a16banner.png" />
</p>

### Introducing Project Elixir now based on Android 16 シ
> <p>"Redefine Simplicity with your android experience on our minimalistic custom rom — where sleek design meets robust security, performance, and stability."</p>

### ⊀ Unleash Innovation ⊁

> Elevate your user interface with minimalist design and with the striking of perfect balanced customization options, customize with ease.

### Installation Guide for Redmi Note 7 Pro (violet)

> [!CAUTION]
> - Your warranty is void. Or valid, probably?
> - Project Elixir is not responsible for any damage you made to your device. You have been warned!
> - Don't fall for mod/cracks etc and you may end up in trouble, in such scenarios you are not to blame us.

> [!Warning]
> * We are not responsible for anything that may happen to your phone by installing custom ROMs.
> * We are not responsible for anything that may happen to your phone by installing any kernels.
> * You do it at your own risk and take the responsibility upon yourself
> * You are not to blame Project Elixir or its respected developers for any of your loss.
> * Be careful while going through download, installation guide, changelog links as A12 = v2.0 (snow), A13 = v3.0 (Tiramisu) and A14 = v4.0 (UNO), A15 = 5.0 (vany) and A16 = v6.0 (bkl) respective branch.

> [!Tip]
> **Basic Notes for all users:**  
> * The provided instructions are for Project Elixir based on Android 16.
> * These will only work if you follow every section and step precisely
> * Do not continue after something fails! Contact in support group for help
> * The device must have an unlocked bootloader & has Platform Tools installed in pc.
> * If you are moving from any other Android version to Android 16, it is necessary to do CLEAN FLASH (Format Data)
> * Take a backup for safe side (If you are coming from older Android version or doing a clean flash)
> * For any queries or help related to Elixir, join our support group : [Tap Here](https://telegram.me/Elixir_Discussion)  

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 16 ]:** [TWRP Recovery](https://www.pling.com/p/1623145/)

3. Download the Project Elixir ROM for Redmi Note 7 Pro aka Violet from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/violet)

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

### Step 3: Flash Recovery using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:
```
fastboot devices
```
> [!Note] 
> - If your device is listed, you are ready to flash the TWRP Recovery.
2. Download the TWRP Recovery ZIP (`.img` file will be in zip) from the link provided in Step 1.
3. Place the downloaded TWRP Recovery image (`.img` file) in the same location as the platform-tools folder on your computer.
4. Now, flash the TWRP Recovery using the following command:
```
fastboot flash recovery recovery_file_name.img
```
> [!Important]
> Replace `recovery_file_name.img` with the actual name of the TWRP Recovery image you downloaded if needed.
5. After flashing the recovery, use the following command to reboot your Recovery:
```
fastboot reboot recovery
```
6. Your device will reboot with Recovery installed.

### Step 4: Wipe Data
1. In TWRP Recovery, use the touch screen or physical buttons to navigate.
2. Select "Wipe" from the main menu.
3. Wipe Data and Davlik & cache and then proceed to format data by typing yes. And reboot to recovery again.

### Step 5: Flash Project Elixir ROM

**Retrofit Dynamic Partitions** `(v5.0 and above versions)` - Clean Flash
```
- Download the latest build (Need to clean flash if you are on Android 14)
- Take a backup for safe side (If you are coming from Android 14 you need to do a clean flash)
- Flash provided recovery Retrofit Supported Recovery from link [Same like step 3]
- Boot to Retrofit Supported Recovery 
- Wipe Data by going to "Factory reset" section in recovery (only click Format data/factory reset)
﻿﻿- Wipe only Dalvik,cache and data (Only these 3 if coming from dynamic) else wipe system too if coming from legacy
﻿﻿- Flash or sideload the ROM zip and Format data
- If you want to be decrypted and want to stay decrypted then flash DFE v5
- Reboot System
```

**Retrofit Dynamic Partitions** `(v5.0 and above versions)` - Dirty Flash
```
- Boot to Retrofit Supported Recovery
- Wipe only Dalvik/cache
- Flash or sideload the ROM zip
﻿﻿- If you are already decrypted then only flash DFE v5 else skip it
- Reboot System
```

Decrypted to Decrypted `(Android 16 to Android 16)`
```
1. Download the Latest Build
2. Boot to Android 16 recovery
3. Clear Dalvik and Cache in advance wipe
3. Flash ROM zip
4. Flash Fcrypt DFE v5 (Compulsory)
5. Reboot
```
> [!Warning]
> **NOTE: All builds are now based on Retrofit Dynamic Partitions from v5.0 or above**

> [!Important]
> **May Required Files:**
> * Retrofit Supported Recovery : [Tap Here for link](https://www.pling.com/p/1623145/)
> * DFE v5.zip : [Tap Here for link](https://www.pling.com/p/1623145/)


> [!Note] 
> **Notes specific to device build**
> * Firmware and Gapps are already included in zip no need to flash additionally
> * If you are coming from ports or HentaiOS you need to Format Data and flash latest firmware
> * If you are coming from Android 12 or 13 to Android 16 then clean flash is compulsory and format data.
> * If you are encrypted do format Data before flashing build to avoid bugs.

<br>

> [!Important]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)

<p align="center">
  <img src="https://github.com/Project-Elixir/docs/blob/bkl/res/elixir-copyright.png" />
</p>
