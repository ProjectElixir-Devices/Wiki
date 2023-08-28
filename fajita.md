![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For OnePlus 6T (fajita)

# Clean Flash
*Back up anything you want to keep from the phone's internal storage to your computer/cloud storage, because we're going to format the userdata partition in this process.*
Download rom zip to computer.
Extract boot.img from rom zip.
Reboot phone to bootloader.
Flash boot image to both slots ('fastboot flash boot_a boot.img' then 'fastboot flash boot_b boot.img').
Reboot phone to bootloader.
Use vol +/- keys to select recovery mode & press power button to enter recovery.
On phone, choose "Apply update" > "ADB sideload" & then from computer, 'adb sideload path/to/rom.zip' (substituting the actual path to the actual filename) to sideload the installation zip; the recovery header graphic will disappear until the process has completed ("error" messages like "no error", or finishing at 47% on the computer are normal).
On phone, choose "Factory reset / Wipe data", and confirm (note: this will erase everything from the phone's internal storage; make sure that you have backed up anything you want to keep first!). If you want to try out f2fs as a filesystem for userdata, give it a shot. It should be stable. If you don't know, just pick ext4; that's what we've been using forever.
On phone, choose "Advanced" > "Reboot recovery" to reboot into recovery on the newly-flashed slot.
Reboot into system.

# OTA Update
Use the built-in Updater ("Settings > System > Updater") to apply OTA updates as they become available, or to manually flash a ROM zip by going to the three-line menu in the upper right and choosing "Local update"
