![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png "Installation")

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

# Easy Installation Guide for Project Elixir on Veux/Peux

This guide will walk you through the process of installing Project Elixir on your Veux/Peux device.

## Before You Begin: Back Up Your Data
Before you start the installation process, it's a good idea to back up your important data to prevent any data loss during the installation.

## 1. Download Necessary Files
To get started, you'll need to download the required files for the installation:

- [boot.img](https://www.pling.com/p/2127492/)
- [vendor_boot.img](https://www.pling.com/p/2127492/)
- [rom.zip](https://www.pling.com/p/1879508/)

## 2. Flash Recovery
Follow these steps to flash the necessary recovery images using ADB:

> [!Important]
> If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options.

1. Connect your device to your computer.
2. Open a command prompt or terminal on your computer.
3. Navigate to the directory where you've downloaded the recovery images.
4. Run the following commands:
```
fastboot flash boot boot.img
```
```
fastboot flash vendor_boot vendor_boot.img
```
```
fastboot reboot recovery
```

#
## 3. Install Project Elixir ROM
Now it's time to install the Project Elixir ROM on your device:

1. In recovery mode, select "Apply Update."
2. Choose "Apply Update from SD Card or OTG."
3. Locate and select the `rom.zip` file you downloaded.
4. Confirm and start the flashing process.
5. Once the flashing is complete, reboot back into recovery.
6. Again, select "Apply Update from SD Card or OTG."
7. If you're doing a clean installation, select "Format Data." (Skip this step if you're doing a dirty flash.)
8. Reboot your device into the system.

## 4. Alternative Installation Method (ADB Sideloading)
Alternatively, you can use ADB sideload method to install the ROM:

1. In recovery mode, select "Apply Update."
2. Choose "Apply Update from ADB."
3. Connect your phone to your PC.
4. Open a command prompt or terminal on your PC.
5. Run the following command:
```
adb sideload rom.zip
```

6. Once sideloading is done, reboot back into recovery.
7. Format Data.
8. Reboot your device into the system.

## 5. Enjoy Project Elixir
Congratulations! You've successfully installed Project Elixir on your Veux/Peux device. Enjoy the new features and customization options that the ROM offers.

Remember, if you encounter any issues during the installation process, feel free to seek help from the Project Elixir community or refer to their official documentation. Happy exploring!
