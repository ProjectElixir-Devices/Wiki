![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on //Nothing Phone 2 (Pong)//

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
   - **Recovery Link [ For Android 14 ]:** [Recovery](https://projectelixiros.com/download)

3. Download the Project Elixir ROM for Nothing Phone 2 aka Pong from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/download)

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
2. Download the Recovery.img from the link provided in Step 1.
3. Place the downloaded Recovery image (`.img` file) in the same location as the platform-tools folder on your computer.
4. Now, flash the Recovery using the following command:
```
fastboot flash recovery recovery.img
```

5. After flashing the recovery, use the following command to reboot your Recovery:
```
fastboot reboot recovery
```
6. Your device will reboot with Recovery installed.

### Step 4: Flash Project Elixir ROM

**- Clean Flash(Sideload Method)**
```
1. Perform a factory reset and return to recovery main mode.
2. Select "Install update" >> "ADB sideload" and sideload the build using the command below:
 
   adb sideload <mention build name>.zip
   Example: adb sideload ProjectElixir_4.1_Pong-14.0-20240229-1326-OFFICIAL.zip
3. Reboot system.
```

**- Clean Flash(Fastboot Method)**
```
1. Boot into bootloader/fastboot mode by Holding down the Power+Volume Down keys.
2. Connect you device and open Command Prompt/Windows terminal.
3. Execute the following command for flashing the ROM:

fastboot -w
fastboot update --skip-reboot path/to/ProjectElixir_.zip

Example: fastboot update --skip-reboot ProjectElixir_4.1_Pong-14.0-20240229-1326-OFFICIAL.zip

4. Enter Recovery.
5. Go to Wipe Data \ Factory Reset to format.
6. Reboot to System.
```

**- Dirty Flash(Sideload Method)**
```
1. Boot into recovery mode.
2. Select "Install update" >> "ADB sideload" and sideload the build using the command below:
 
   adb sideload <mention build name>.zip
   Example: adb sideload ProjectElixir_4.1_Pong-14.0-20240229-1326-OFFICIAL.zip
3. Reboot system.
  
                                  OR

Just update through the system updater.
```
> [!Important]
> You must be on Elixir Recovery to be able to update from system updater.
 

**- Dirty Flash(Fastboot Method)**
```
1. Boot into bootloader/fastboot mode by Holding down the Power+Volume Down keys.
2. Connect you device and open Command Prompt/Windows terminal.
3. Execute the following command for flashing the ROM:

fastboot update path/to/ProjectElixir_.zip

Example: fastboot update ProjectElixir_4.1_Pong-14.0-20240229-1326-OFFICIAL.zip
```

> [!Important]
> **May Required Files:**
> * Android 14 Recovery Link : [Tap here for link](https://projectelixiros.com/download)
> * Any Extra File link if required : [Tap Here for link](https://sourceforge.net/projects/project-elixir/files/fourteen)

<br>

> [!Note] 
> **Notes specific to device build**
> * Gapps is already included in zip no need to flash additionally
> * If you are coming from PORTs then you need to Format Data and flash latest firmware [depending on the device]
> * If you are coming from Android 12 or 13 to Android 14 then clean flash is compulsory and format data.

<br>

> [!Important]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)