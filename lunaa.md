![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For Project Elixir on lunaa(RMX3360-RMX3363)

!! CLEAN FLASH ONLY !!
Step 1 (Firmware flashing):
!!SKIP THIS STEP IF YOU ARE ON F.01, F.02, F.03 OR F.04 FIRMWARE. GO TO STEP 2!!
• Backup all your data.
• Disable driver signature enforcement (Google this.)
• Install 15s ADB drivers
• Reboot your PC/laptop
• Connect phone to PC
• Download the recovery (https://t.me/elixir_gtme/13698)
• Extract the recovery
• Flash the recovery in bootloader, but don't reboot.
• Then download F.01 firmware (https://t.me/elixir_gtme/13858)
• Extract the firmware into a folder

• Open a terminal in the folder
• Type fastboot devices (If your serial number comes up and fastboot next to it, your ready for next step. If fastboot devices returns nothing, google your issue to solve it.)
• Type fastboot reboot fastboot and hit enter (You will reboot to fastbootd.)
• Type fastboot devices again to confirm that everything is working
• Then type flash_all.bat (or .sh if your on linux) and hit enter. The firmware flashing process will begin.
• Then reboot to bootloader and follow from step 2.

Step 2 (Sideloading the rom):
• If you skipped step 1, please reboot your device to bootloader.
• Type fastboot reboot fastboot and hit enter.
• Then type fastboot -w and hit enter.
• Then reboot to recovery.
• Then, sideload the Elixir package.
• After it has finished, reboot and enjoy!
