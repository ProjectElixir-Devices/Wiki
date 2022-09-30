![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For Project Elixir on Munch
- Reboot device into fastboot mode.
- Flash the recovery.img provided -cmd fastboot flash boot <recovery.img>.
- Reboot device into recovery -cmd fastboot reboot recovery or press volume-up + power button.
- Format/factory reset.
- Sideload rom.zip -cmd adb sideload <rom.zip>.
- Reboot.

### Note:
- Firmware is inbuilt.
- Clean flash is compulsory if coming from a12. Can dirty flash if coming from a13 initial build.
- Use Twrp or orange fox recovery.