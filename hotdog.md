![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on OnePlus 7T Pro (hotdog)

### **Note:**  - Make sure you are using Oxygen OS 11 (v11.0.9.1) -
The device must have an unlocked bootloader. If you are moving from
Android 9/10/11/12/13 to Android 14, it is necessary CLEAN FLASH (Format
Data).

### Step 1: Download Required Files 
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [TWRP Recovery](https://dl.twrp.me/hotdog/twrp-3.6.2_11-0-hotdog.img.html)

3. Download the Project Elixir ROM for OnePlus 7T Pro aka hotdog from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/hotdog)

4. Download Firmware zip from link below:
   - **Oxygen OS 11 (v11.0.9.1) Link**: [Download Firmware](https://drive.google.com/file/d/1RDts_laWjRQ8zE550KWFwZskfOmpIVJF/view)

### Step 2: Install ADB and Boot into Fastboot Mode 
1. Make sure you have ADB (Android Debug Bridge) installed on your computer.

2. Extract the downloaded platform-tools zip file on your computer.

3. Connect your device to your computer using a USB cable.

4. Open a command prompt (Windows) or terminal (macOS and Linux) on your computer.

5. Navigate to the location where you extracted the platform-tools.

6. Enter the following command to check if your device is connected and detected by ADB:

```
adb devices
```

If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options.

7. Now, reboot your device into Fastboot Mode using the following command:

```
adb reboot bootloader
```

### Step 3: Unlock Bootloader using Fastboot Mode 
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:

``` 
fastboot devices
```

2. If your device is listed, you are ready to unlock by using following cmd

``` 
fastboot oem unlock
```

3. Place the downloaded twrp-3.6.2_11-0-hotdog.img in the same location as the platform-tools folder on your computer.

4. Now, boot to recovery using the following command:

``` 
fastboot boot twrp-3.6.2_11-0-hotdog.img
```
5. After this your device will boot to recovery

### Step 4: Clean Flash Project Elixir

- Download the latest Project Elixir build
- Make sure you are using [Oxygen OS 11
(v11.0.9.1)](https://drive.google.com/file/d/1RDts_laWjRQ8zE550KWFwZskfOmpIVJF/view)
- Take a backup for safe side.
- Boot to TWRP mention in Step 1 for OOS 11.
- Wipe Dalvik/Cache + Data + Metadata.
- Reboot to TWRP.
- Flash the ROM. 
- Reboot to system.

### Dirty Flashing Steps 

**NOTE:** After you flash Elixir A14, TWRP is no longer supported.

- Reboot to Elixir Recovery.
- Sideload the new update.
- Reboot to system.

OR

- Perform a local update from the Updater.

### Notes: 
- The ROM comes with GApps inbuilt.
- If you are coming from A12/A13 to A14, then a clean flash is a must.
- Clean flash is always recommended to get the best experience.
