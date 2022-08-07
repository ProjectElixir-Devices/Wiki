![Installation Guide For Project Elixir on Violet](https://i.imgur.com/5PIB1RV.jpg "Installation")

# Installation Guide For Project Elixir on guacamole

## IF YOU ARE MOVING FROM ANOTHER ROM, CLEAN FLASH Is COMPULSORY.

**--- Clean Flash ---**
 - Extract ```boot.img``` from device or stock Android 11 firmware
   - use https://github.com/ssut/payload-dumper-go to extract from stock firmware
 - Reboot to fastboot
   - flash boot.img  ```fastboot flash boot boot.img```
 - Reboot to Recovery
   - sideload rom ```adb sideload <ROM_FILE_NAME>```
 - Reboot to system

**--- Dirty Flash ---**
- Download the latest build
- Reboot to recovery
- Flash the latest build | adb sideload PixelPlusUI_4.1_guacamole-12.0-20220116-1639-OFFICIAL.zip
- Wipe Cache
- Reboot :p
