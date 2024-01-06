![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

## Installation Guide for Project Elixir on Google Pixel 2XL (Taimen) 

### Basic requirements
1. Read through the instructions at least once before actually following them, so as to avoid any problems due to any missed steps!
2. Make sure your computer has adb and fastboot
3. Enable USB debugging on your device
4. Boot your device with the stock OS at least once and check every functionality. Make sure that you can send and receive SMS and place and receive calls (also via WiFi and LTE, if available)

### Unlocking the bootloader
1. Enable OEM unlock in the Developer options under device Settings, if present
2. Connect the device to your PC via USB
3. On the computer, open a command prompt (on Windows) or terminal (on Linux or macOS) window, and type:
```
adb reboot bootloader
```
   - You can also boot into fastboot mode via a key combination with the device powered off, hold Volume Down + Power
4. Once the device is in fastboot mode, verify your PC finds it by typing:
```
fastboot devices
```
   If you get any output or an error:
   - on Windows: make sure the device appears in the device manager without a triangle. Try other drivers until the command above works!
   - on Linux or macOS: If you see no permissions fastboot try running fastboot as root. When the output is empty, check your USB cable and port!
5. Now type the following command to unlock the bootloader:
```
fastboot flashing unlock
```
6. If the device doesn’t automatically reboot, reboot it. It should now be unlocked.
7. Since the device resets completely, you will need to re-enable USB debugging to continue.

### Repartition
Specially for Project Elixir A14, you must repartition again your device. If you have repartitioned with partition A13, well you just need to flash the new repart file, no need to back to the stock partition again.

1. Download [TWRP Recovery](https://github.com/Google-Pixel2-2XL/instalation_guide_wahoo/raw/evolution-x/taimen/twrp/twrp-3.7.0_9-0-taimen.img)
2. Download [productpartition-taimen-a14.zip](https://github.com/Google-Pixel2-2XL/instalation_guide_wahoo/raw/evolution-x/taimen/repart/productpartition-taimen-a14.zip)
3. Connect your device to your PC via USB if it isn’t already.
4. If your device isn’t already in fastboot mode, on the computer, open a command prompt (on Windows) or terminal (on Linux or macOS) window, and type:
```
adb reboot bootloader
```
5. Once the device is in fastboot mode, verify your PC finds it by typing: 
```
fastboot devices
```
6. Flash the TRWP Recovery on your device by typing:
```
fastboot flash boot <recovery_filename>.img
```
   - Replace <recovery_filename> with the actual filename or just drag & drop the file to the terminal
7. Now reboot into recovery
8. Sideload the new partition file by typing:
```
adb sideload <partition_filename>.zip
```
   - Replace <partition_filename> with the actual filename or just drag & drop the file to the terminal
   - On the TWRP Recovery, select "Advance", "Adb sideload", then swipe to begin sideload
9. After flash complete, on TWRP select return to the main menu
10. Now tap Wipe, then select Format data/factory reset and continue with the formatting process.

## Flashing

### Clean flash
1. Reboot to bootloader by typing:
```
adb reboot bootloader
```
2. Wipe data by typing:
```
fastboot -w
```
3. Flash TWRP or boot.img provided
4. Reboot to recovery
  - On the TWRP Recovery, select "Advance", "Adb sideload", then swipe to begin sideload
  - On the Elixir Recovery, select "Apply update"
5. Sideload the ROM by typing:
```
adb sideload <ROM_filename>.zip
```
  - Replace <ROM_filename> with the actual filename or just drag the file to the terminal
6. Reboot system

### Dirty flash
1. Reboot to recovery by typing:
```
adb reboot recovery
```
  - On the Elixir Recovery, select "Apply update"
2. Sideload the ROM by typing
```
adb sideload <ROM_filename>.zip
```
  - Replace <ROM_filename> with the actual filename or just drag the file to the terminal
3. Reboot system

## Note:
If you want to back to the stock partition table, kindly download and flash the this [Stock Partiton - Pixel 2 XL](https://github.com/Google-Pixel2-2XL/instalation_guide_wahoo/raw/evolution-x/taimen/repart/stockpartition-pixel2xl.zip)