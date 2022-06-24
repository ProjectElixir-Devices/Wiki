# Installation for OnePlus 9 Pro (lemonadep)

1. Download the .ZIP folder that contains dtbo, vendor_boot, and boot:https://android.redbirdvirtual.com/Lemonadep%20%28OnePlus%209%20Pro%29/Image%20Files/
2. Reboot to bootloader and flash dtbo (fastboot flash dtbo dtbo.img)
3. Flash vendor_boot (fastboot flash vendor_boot)
4. Flash boot (fastboot flash boot.img)
5. Reboot to Recovery Mode (fastboot reboot recovery)
6. Select "Apply update from ADB."
7. 'adb sideload rom.zip'
8 Do Factory reset/format data from recovery
9. Restart to system
