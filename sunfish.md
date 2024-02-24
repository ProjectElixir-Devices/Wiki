![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Google Pixel 4a (sunfish)

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
> [!Important]
> - If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options
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

  ### Enjoy Project Elixir
> - Congratulations! You've successfully installed Project Elixir on your device
> - Enjoy the new features and customization options that the ROM offers
> - Remember, if you encounter any issues during the installation process, feel free to seek help from the Project Elixir community or refer to their official documentation.

> [!Important]
> **May Required Files:**
> - A14 boot image: [Tap here for link](https://www.pling.com/p/1980617/)


> [!Note] 
> **Notes specific to device build**
> * Gapps is already included in zip no need to flash additionally
> * If you are coming from Android 12 or 13 to Android 14 then clean flash is compulsory and format data.
> * If you are encrypted do format Data before flashing build to avoid bugs.
