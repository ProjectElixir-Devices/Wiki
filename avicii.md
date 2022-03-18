![Installation Guide For Project Elixir on Avicii](https://i.imgur.com/5PIB1RV.jpg "Installation")

# Installation Guide For Project Elixir on Avicii

## IF YOU ARE MOVING FROM ANDROID 10 or ANDROID 11 TO ANDROID 12 then CLEAN FLASH ( Format Data ) Is COMPULSORY.


### Unlocking Bootloader : 
1. Backup everthing before doing anything (Swift Backup recommended, needs rooted phone tho)
2. Remove Screen lock security
3. Install Adb drivers, qualcomm drivers and fastboot drivers in PC
4. Download Platform Tools
5. Run CMD in PLatform Tools Directory
6. Finsih up Fastboot installations
7. OEM unlock, Bootloader unlock
   1. Turn on developer settings
`  2. Turn on OEM unlock, USB debugging
   3. Reboot to FASTBOOT
8. ### Run commands:-
   1. fastboot devices
   2. fastboot flashing unlock
   3. Use volume buttons to navigate and Unlock Bootloader
   4. It will wipe your data and reboot your system. 
9. Do offline setup. 
10. Turn on Developer options
11. Turn on USB debugging
12. Run "adb devices" on CMD in PlatformTools Directory and authorise the device

### Installing the Rom: 
1. Reboot to Bootloader
2. Download AOSP Recovery or PEX Recovery(stable version of your Device and Android version respectfully and place them in PlatformTools Diretory)
3. ### Run command:-
  1. fastboot devices
  2. fastboot boot (Any recovery name).img
4. It will boot into the recovery image
5. Tap on Update, update from ADB sideload
6. Download and custom ROM zip file and place it in the PlatformTools Diretory
7. ### Run Command:-
   1. adb sideload (Name of the Rom).zip
8. If it fails, tap on advanced, reboot to bootloader and try the other recovery
9. The installation takes upto 10 mins, and fails exactly at 47%
10. Factory reset in the recovery image
11. Reboot to System
12. Hopefully you're all set with a new ROM of your choice
