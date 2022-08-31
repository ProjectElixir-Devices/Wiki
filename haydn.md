![68747470733a2f2f692e696d6775722e636f6d2f33556d4b366e532e706e67](https://user-images.githubusercontent.com/107272205/187671893-513b8818-67b0-4ebc-9b46-66a131616c7e.png)

### Installation Guide For Project Elixir on Haydn
- Reboot device into fastboot mode.
- Flash the recovery.img provided -cmd fastboot flash boot <recovery.img>.
- Reboot device into recovery -cmd fastboot reboot recovery or press volume-up + power button.
- Format/factory reset.
- Sideload rom.zip -cmd adb sideload <rom.zip>.
- Reboot.

### Note:
- Firmware is inbuilt no need to flash again.
- Clean flash is compalsary if coming from a12-a13.
