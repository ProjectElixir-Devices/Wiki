![Installation Guide For Project Elixir on sweet](https://i.imgur.com/Hb3gl9Q.jpg "Installation")

# Installation Guide For Project Elixir on sweet

## IF YOU ARE MOVING FROM ANDROID 10 or ANDROID 11 TO ANDROID 12 then CLEAN FLASH ( Format Data ) Is COMPULSORY.

## Recovery Link : [TWRP Recovery](https://build.twrp.me/twrp-3.6.0_11-0-sweet.img)

# Flashing Custom Recovery using PC 
Guide to flash recovery on Redmi Note 10 Pro / Pro Max
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

## Installation Guide For Project-Elixir on sweet

## About ROMs
We have two types of Custom ROMs on the Redmi Note 10 Pro / Pro Max

• MIUI Vendor Based ROM

• OSS Vendor Based ROM

## What is OSS vendor?
• OSS (which stands for open-source software) vendor allows the developers to modify the vendor to remove MIUI bloat from the vendor and fix any issues by directly modifying the vendor, instead of overlaying it.

## A few things to keep in mind
• Before flashing a MIUI vendor-based ROM, make sure you are on the correct vendor/firmware for YOUR region. You can get flashable ZIPs here so you do not have to the flash MIUI before flashing the ROM (Thanks @grewal) This means, if you have an Indian device variant, flash the with the latest vendor/firmware for India (sweetin). Flashing the wrong vendor will cause different issues such as worse battery drain (due to NFC spam), a green/blue tint in camera (as the Global markets do not have the 64MP device, using that vendor on the 64MP variant will cause such issues)

• If you shift from a MIUI vendor-based ROM to another MIUI vendor-based ROM or to an OSS vendor-based ROM, you do not have to flash the vendor again. However, if you want to switch from an OSS vendor-based ROM to a MIUI vendor-based ROM, you will need to flash the right vendor/firmware for your region.

## Project-Elixir Based OSS Vendor Or MIUI Vendor ?

• Well Project-Elixir Based On OSS Vendor.


## A few notes about flashing Custom ROMs
• This is a device with dynamic partitions.

• You should NOT wipe any partition to clean flash a ROM.

## Flashing MIUI vendor-based ROMs
• Make sure you are on the latest vendor/firmware for YOUR region. (You will only need to reflash if coming from an OSS vendor ROM)

• Flash the ROM

• Flash GApps (Optional if flashing a vanilla ROM which means GApps are not included)

• Format Data (Not the same as wiping data)

TWRP: Wipe > Format Data > Type "yes" & enter
OFOX: Menu > Manage Partitions > Data > Format Data > Type "yes" & enter
• Reboot to system

## Flashing OSS vendor-based ROMs
• Flash the ROM

• Flash GApps (Optional if flashing a vanilla ROM which means GApps are not included)

• Format Data (Not the same as wiping data)

TWRP: Wipe > Format Data > Type "yes" & enter
OFOX: Menu > Manage Partitions > Data > Format Data > Type "yes" & enter
• Reboot to system

## About DFE (Disable Force Encryption)
It is strongly advised to not use this! Anyone with physical access to your phone (for example if lost or stolen) can get all your confidential data, including photos and even saved passwords, and makes identity theft possible.

Whenever possible, back up your data and do a proper encrypted setup!
