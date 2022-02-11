![Installation Guide For Elixir on ysl]
# Flashing Custom Recovery using PC 
Guide to flash recovery on Redmi Y2
Requirements:
• A computer
• Unlocked bootloader
• Ability to use brain

Steps:
1. Download the following files-
• [Platform Tools](https://developer.android.com/studio/releases/platform-tools)
2. Copy custom recovery and  to platform tools.
3. Boot your phone into fastboot mode and connect it to your computer.
4. Open command prompt in platform tools directory and type the following commands-

fastboot flash recovery recoveryname.img

fastboot reboot recovery

Done, happy flashing :)

## Installation Guide For Elixir on ysl

### MIUI to Elixir
1. After flashing custom recovery, boot to recovery.
2. Go adv. wipe :- wipe [dalvik, cache, system, vendor ,data]
3. Format data (By typing yes)
4. Reboot to recovery.
5. Flash rom.
6. Reboot system.

### A different Rom to Elixir
1. Reboot to recovery.
2. Go adv. wipe :- wipe [dalvik, cache,system,vendor,data ]
3. Reboot to recovery.
4. Flash rom.                          
5. Reboot system.
                   
### Elixir(OLD VERSION) to Elixir(NEW VERSION)
1. Reboot to recovery.
2. Go adv. wipe :- wipe [dalvik, cache, ]
3. Flash new version of Elixir.
4. Reboot system.
