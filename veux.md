![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png "Installation")

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