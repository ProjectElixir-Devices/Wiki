![Installation Guide For Project Elixir on Xiaomi MI A3](https://i.imgur.com/Hb3gl9Q.jpg "Installation")

# Installation Guide For Project Elixir on Xiaomi MI A3 


### CLEAN FLASH GUIDE
You MUST have unlocked bootloader and android 11 firmware on your phone
1) Flash LineageOS recovery via fastboot
fastboot flash boot <name of the recovery img file>.img
(get it by #los_recovery_img)
2) Reboot to recovery.
3) Perform factory reset.
4) Navigate Apply update -> apply from ADB
5) Sideload rom .zip .
adb sideload <rom zip name> or if you have sd card or otg just copy the rom in that and flash through sd card or otg
6) follow the same process to flash los recovery zip (the same way how u flashed rom zip)
7) Reboot System and Enjoy.

### DIRTY FLASH GUIDE
1. Reboot to Recovery.
3. Flash Project Elixir Rom.
4. Wipe Dalvik, Cache.
5. Reboot to System.

## Notes:
- Clean flash is must if coming from miui or different roms.