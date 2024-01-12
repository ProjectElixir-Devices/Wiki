![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Fajita

###  **Note:** 
- The device must have an unlocked bootloader. If you are moving from Android 13 to Android 14, it is necessary to install stable OOS firmware and perform a CLEAN FLASH (Format Data).

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download Elixir Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [DOWNLOAD](https://www.pling.com/p/1866093/)

3. Download the stable OOS firmware from the link below:
   - **Firmware Link**: [OOS Firmware](https://download.h2os.com/OnePlus6T/MP/OnePlus6THydrogen_34.K.62_OTA_0620_all_2112282145_db7672c020714abb.zip)

4. Download the Project Elixir ROM for Fajita from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/download)

5. Download this super_empty.img file
   - **super_empty.img**: [DOWNLOAD](https://sourceforge.net/projects/project-elixir/files/fourteen/fajita/super_empty/)

6. Download this vbmeta.img file
   - **vbmeta.img**: [DOWNLOAD](https://sourceforge.net/projects/project-elixir/files/fourteen/fajita/vbmeta/)

### Step 2: Initializing Dynamic partitions
1. Download super_empty.img file
2. Power off the device, and boot it into bootloader mode
3. Flash vbmeta.img with the following commands:
```
fastboot flash vbmeta_a vbmeta.img
fastboot flash vbmeta_b vbmeta.img
```
4. Flash ProjectElixir Recovery:
```
fastboot flash boot boot.img
```
5. Erase the old android partitions with the following commands:
```
fastboot erase system_a
fastboot erase system_b
fastboot erase odm_a
fastboot erase odm_b
fastboot erase vendor_a
fastboot erase vendor_b
```
6. Now reboot into recovery and enter fastbootd mode
7. Initialize the retrofit super partitions for each slot:
```
fastboot wipe-super super_empty.img
fastboot set_active other
fastboot wipe-super super_empty.img
fastboot set_active other
```
8. Choose Enter recovery to return to recovery

### Step 3: Flash Project Elixir ROM from recovery
1. Download Project Elixir Rom Package.
2. If you are not in recovery, reboot into recovery [hold Volume Down + Power]
3. Now tap Factory Reset, then Format data / factory reset and continue with the formatting process. 
- This will remove encryption and delete all files stored in the internal storage, as well as format your cache partition (if you have one)
4. Return to the main menu.
5. Sideload the Project Elixir Rom.zip package:
6. On the device, select “Apply Update”, then “Apply from ADB” to begin sideload.
- On the host machine, sideload the package using:
```
adb sideload Rom.zip.
```
7. Once you have installed everything successfully, click the back arrow in the top left of the screen, then “Reboot system now”.

###  **Note:** 
- The first boot usually takes no longer than 15 minutes, depending on the device.
- If the installation process reports the message "(~47%)
```
adb: failed to read the command: No error
```
do not worry, the process was completed successfully and you can restart the device
