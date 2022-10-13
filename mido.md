Android 13 Release Notes/Installation Guide

1. Clean Flash 
• Clean flash is mandatory: you are required to backup all of your existing data to your computer or your preferred cloud service and avoid using nandroid backup.
Seedvault backup not working yet

2.Flash TWRP
• Flash the new TWRP Recovery made by Zeelog : ( Mandatory)due to various changes in fstab file and encryption implementation, you are required to flash the new TWRP of which the link is undermentioned 

Link (https://github.com/zeelog/device_mido_twrp/releases/download/2.0/twrp_3.7.0_12-0-mido.img) 

3. Wipe and format Device ( Both are different)
• After you flash and boot into the new TWRP recovery, format data and reboot to the recovery again. 
Now, wipe all the partitions (i.e. system, vendor, data, internal storage). Wiping Internal might throw an error because of missing /data/media/ which is okay, reboot to recovery again.  
This format data and wiping of other partitions is required only once every clean flash.
NB : encryption is now enabled by default and that is why a clean flash would cost you a data format.

4.Flash ROM and Gapps
*To use internal storage for transferring files from PC 

From TWRP > tap Advanced > Terminal > run command:
mkdir -p /data/media/0/

• Copy the latest releases Project Elixir Android 13 rom to your internal storage/otg media/sd card etc. 
Flash the ROM using the usual method.

6.Go Back 
If you want to go back to the previous ver of Android. 
You need to flash your old recovery and Wipe and Format device ,Flash ROM again.

=============================================

* FOR Video Guide: https://t.me/LOSRN4/284718

=============================================
