![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Nothing Phone 1 (Spacewar)

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
   - **Recovery Link [ For Android 14 ]:** [Download Recovery](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/recovery/)

3. Download the Project Elixir ROM for Nothing Phone 1 (Spacewar) from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/Spacewar)

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

### Step 2: Unlock your bootloader [skip to next step if you already]
> [!Warning] 
> **DISCLAIMER**
> - After unlocking the bootloader, all of your data will be erased, so create a backup of your important data before proceeding.
> - Unlocking may break or modify some system functions and might prevent you from updating the system version.
> - Your warranty will be void. 
> - If you end up bricking your device, if not followed the instructions carefully or anything unusual happens to your device during this process, then no one except you will be responsible for it.

1. Open Platform Tools folder > click on the address bar > type CMD > hit Enter
2. Write this command 
```
adb devices
``` 
3. Allow the PC to connect to the phone using USB and
4. Now, reboot your device into Fastboot Mode using the following command: 
```
adb reboot bootloader 
```
5. Now start unlocking your device using the following command: 
```
fastboot flashing unlock
```
and
```
fastboot flashing unlock_critical
```
6. After this, your phone will reboot and automatically wipe your data.

> [!Important]
> - If you have encountered some problems, feel free to ask for help at : Nothing Phone (1) | Global 

### Step 4: Boot to Fastboot and flash recovery
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:
```
fastboot devices
```

> [!Important]
> - Download Boot : [Boot Img](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/recovery/) 
> - Download Vendor : [Vendor_Img](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/vendor/)
> - Flash these files through fastboot

2. Now, in fastboot mode start flashing recovery using the following command:
```
fastboot flash boot ./boot.img
```
3. Now start flashing vendor img using the following command:
```
fastboot flash vendor_boot ./vendor_boot.img
```
4. After flashing above images, Reboot to Recovery.
```
fastboot reboot recovery
```
5. After this your device will boot to recovery

### Step 5: Boot into Elixir Recovery and flash ROM

- Factory reset > Format data/factory reset
- Back to recovery home page & Apply update > Apply from ADB
- Open command prompt & sideload rom using command adb sideload <rom_filename>.zip
- Reboot to system


### Dirty Flash :
1. Boot into fastboot
2. Now, in fastboot mode start flashing recovery using the following command:
```
fastboot flash boot ./boot.img
```
3. Now start flashing vendor img using the following command:
```
fastboot flash vendor_boot ./vendor_boot.img
```
4. After flashing above images, Reboot to Recovery.
```
fastboot reboot recovery
```
5. Back to recovery home page & Apply update > Apply from ADB
6. Open command prompt & sideload rom using command adb sideload <rom_filename>.zip
7. Reboot to system
     
> [!Note] 
> **Notes specific to device build**
> * Rom is Encrypted
> * Firmware and Gapps are already included in zip no need to flash additionally
> * If you are coming from Android 13 to Android 14 then clean flash is compulsory and format data.
> * If you are encrypted do format Data before flashing build to avoid bugs.

<br>

> [!Important]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)
