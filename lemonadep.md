# Installation for OnePlus 9 Pro (lemonadep)

1. Download recovery by tapping on the "recovery" : https://drive.google.com/drive/folders/1-zX-6CD2V4ipp8b3ZNEH3tt9b1mGni0d
2. Reboot to bootloader and flash dtbo (fastboot flash dtbo dtbo.img)
3. Flash vendor_boot (fastboot flash vendor_boot)
4. Flash boot (fastboot flash boot.img)
5. Reboot to Recovery Mode (fastboot reboot recovery)
6. Select "Apply update from ADB."
7. 'adb sideload rom.zip'
8 Do Factory reset/format data from recovery
9. Restart to system
