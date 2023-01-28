![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

## Installation Guide For Project Elixir on Taimen

### Basic requirements
1. Read through the instructions at least once before actually following them, so as to avoid any problems due to any missed steps!
2. Make sure your computer has adb and fastboot.
3. Enable USB debugging on your device.
4. Boot your device with the stock OS at least once and check every functionality. Make sure that you can send and receive SMS and place and receive calls (also via WiFi and LTE, if available), otherwise it won’t work on Project Elixir either!
5. Project Elixir is provided as-is with no warranty. While we attempt to verify e[verything works](https://projectelixiros.com/documentation) you are installing this at your own risk!

### Unlocking the bootloader
1. Enable OEM unlock in the Developer options under device Settings, if present.
2. Connect the device to your PC via USB.
3. On the computer, open a command prompt (on Windows) or terminal (on Linux or macOS) window, and type:
```bash
adb reboot bootloader
```
    You can also boot into fastboot mode via a key combination with the device powered off, hold Volume Down + Power.
4. Once the device is in fastboot mode, verify your PC finds it by typing:
```bash
fastboot devices
```
    If you don’t get any output or an error:
        1. on Windows: make sure the device appears in the device manager without a triangle. Try other drivers until the command above works!
        2. on Linux or macOS: If you see no permissions fastboot try running fastboot as root. When the output is empty, check your USB cable and port!

5. Now type the following command to unlock the bootloader:
```bash
fastboot flashing unlock
```
6. If the device doesn’t automatically reboot, reboot it. It should now be unlocked.
7. Since the device resets completely, you will need to re-enable USB debugging to continue.

### Booting a custom recovery using fastboot
1. Download the [TWRP Recovery](https://dl.twrp.me/taimen/twrp-3.7.0_9-0-taimen.img)
Simply download the latest recovery file.
2. Connect your device to your PC via USB if it isn’t already.
3. If your device isn’t already in fastboot mode, on the computer, open a command prompt (on Windows) or terminal (on Linux or macOS) window, and type:
```bash
adb reboot bootloader
```
    You can also boot into fastboot mode via a key combination Wwith the device powered off, hold Volume Down + Power.

4. Once the device is in fastboot mode, verify your PC finds it by typing: 
```bash
fastboot devices
```
    If you don’t get any output or an error:
        1. on Windows: make sure the device appears in the device manager without a triangle. Try other drivers until the command above works!
        2. on Linux or macOS: If you see no permissions fastboot try running fastboot as root. When the output is empty, check your USB cable (preferably use a USB Type-A 2.0 one or a USB hub) and port!

5. Flash the TRWP Recovery on your device by typing
```bash
fastboot flash boot <recovery_filename>.img
```
(replace <recovery_filename> with the actual filename!)
6. Now reboot into recovery to verify the installation.
    Use the menu to navigate to and to select the Recovery option.

### Pre-install instructions
Starting with Android 12, you must re-partition the device for Project Elixir to be installed.

1. Download [Product Partition 3GB - Pixel 2 XL](https://gitlab.pixelexperience.org/android/vendor-blobs/wiki_blobs_wahoo/-/raw/main/productpartition-pixel2xl-extended.zip)
2. Sideload the .zip package:
    1. On the TWRP Recovery, select ”Advance“, “Adb sideload”, then swipe to begin sideload.
    2. On the computer, type adb sideload and drag to terminal the Product Partition 3GB file then enter
3. Return to the main menu.
4. Now tap Wipe, then Format data / factory reset and continue with the formatting process. Next reboot to recovery again
5. Then sideload the rom like sideloading the Product Partition 3GB on poin nuber 2

Note: If you want to revert to the stock partition table, kindly download and flash the this [Stock Partiton - Pixel 2 XL](https://gitlab.pixelexperience.org/android/vendor-blobs/wiki_blobs_wahoo/-/raw/main/deproduction-pixel2xl.zip)

### Credit:
1. Elixir Project
2. Pixelboot for repart file