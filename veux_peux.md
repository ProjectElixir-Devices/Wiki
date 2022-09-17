![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

# Installation Guide For Project Elixir on Veux/Peux

## IF YOU ARE MOVING FROM ANOTHER ROM, CLEAN FLASH Is COMPULSORY.

### Recovery links
1). [boot](https://sourceforge.net/projects/ashish-builds/files/Recovery-A13//boot.img/download)
2). [vendor_boot](https://sourceforge.net/projects/ashish-builds/files/Recovery-A13/vendor_boot.img/download)

## Flashing Recovery through ADB:
1. fastboot flash boot boot.img
2. fastboot flash vendor_boot  vendor_boot.img
4. fastboot reboot recovery

## Flashing ROM:
### Via SD Card
* Select Apply Update
* Apply Update from SD Card or OTG
* Select rom and flash it
* reboot to recovery again
* Apply Update from SD Card or OTG
* format data(if you make it dirty flash skip this step)
* reboot to system
* Enjoy

Or
### Via ADB Sideload
* Select Apply Update
* Apply Update from ADB
* Connect your phone to PC
* adb sideload rom.zip
* reboot to recovery again
* format data
* reboot to system
* Enjoy
