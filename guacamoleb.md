![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on OnePlus 7 (guacamoleb)

> [!Warning]
> * Your warranty is void. Or valid, probably?
> * Project Elixir is not responsible for any damage you made to your device. You have been warned!
> * We are not responsible for anything that may happen to your phone by installing custom ROMs.
> * We are not responsible for anything that may happen to your phone by installing any kernels.
> * You do it at your own risk and take the responsibility upon yourself
> * You are not to blame Project Elixir or its respected developers for any of your loss.
>
> **Basic Notes for all users:**  
> * The provided instructions are for Project Elixir based on Android 14.
> * These will only work if you follow every section and step precisely
> * Do not continue after something fails! Contact in support group for help
> * The device must have an unlocked bootloader & has Platform Tools installed in pc.
> * If you are moving from any other Android version to Android 14, it is necessary to do CLEAN FLASH (Format Data)
> * Take a backup for safe side (If you are coming from older Android version or doing a clean flash)
> * For any queries or help related to Elixir, join our support group : [Tap Here](https://telegram.me/Elixir_Discussion)  

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 14 ]:** [Elixir Recovery](https://www.pling.com/p/1947572/)

3. Download the Project Elixir ROM for OnePlus 7 (guacamoleb) from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/guacamoleb)
   
### Step 2: Install ADB and boot to fastboot

> [!Important]
> **Note for Unlocking Bootloader**
> - Unlocking the bootloader will erase all data on your device! 
> - You cannot directly unlock the bootloader if you are on latest OxygenOS 12.1. For unlocked bootloader on OxygenOS 12.1, you will need to unlock the bootloader on OxygenOS 11 first and then update to OxygenOS 12.1
> - Before following these instructions please ensure that the device is currently using latest Android 12.1 firmware.

1. Make sure you have ADB (Android Debug Bridge) installed on your computer. 
2. Extract the downloaded platform-tools zip file on your computer.
3. Connect your device to your computer using a USB cable.
4. Open a command prompt (Windows) or terminal (macOS and Linux) on your computer.
5. Navigate to the location where you extracted the platform-tools.
6. Enter the following command to check if your device is connected and detected by ADB:
```
adb devices
```
> [!Important]
> - If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options
> - Enable OEM unlock in the Developer options under device Settings
> - You can also boot into fastboot mode via a key combination: turn the device off, hold `Volume Up + Volume Down + Power`

7. Now, reboot your device into Fastboot Mode using the following command:
```
adb reboot bootloader
```

### Step 3: Unlock Bootloader using Fastboot

1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:
```
fastboot devices
```
2. Your device should appear on the screen. If not then
> [!Note] 
> - **On Windows:** Download latest fastboot driver and copy the folder into your desktop, then go again in Device Manager, locate your device, right-click on your device and choose "Update driver", choose "Browse my computer for driver software", then “Browse…” and select the folder you copied in your desktop. Click “ok” and then on “next”.
> - **on Linux or macOS:** If you see no permissions fastboot try running fastboot as root. When the output is empty, check your USB cable and port!

3. Now type the following command to unlock the bootloader type:
```
fastboot oem unlock
```
> [!Important]
> - At this point the device may display on-screen prompts which will require interaction to continue the process of unlocking the bootloader.
> - Give next/agree to actions the device when it asks you to proceed.
4. If the device doesn’t automatically reboot, reboot it manually.
5. You’ll need to re-enable USB debugging to continue


### Step 3: Flash Elixir Recovery using Fastboot

1. Download ProjectElixir Recovery from this link: [Tap Here](https://sourceforge.net/projects/project-elixir/files/fourteen/guacamoleb/recovery/)
 
> [!Note]
> - If download link doesn’t work we can extract recovery from rom zip file.

**Steps to extract Boot img from ROM zip**
- Download Project Elixir Rom & Download `FastbootEnanche` from this link: [Tap Here](https://github.com/libxzr/FastbootEnhance/releases/download/v1.4.0/Release.zip) and extract it on your desktop
- Open “FastEnanche.exe
- Go into “Payload Dumper” window
- Click on “Browse”
- Select the rom zip you downloaded previously
- Go into “Partitions” window
- Click on boot and then “Extract image”
- You can save it in the same folder as adb & fastboot
 
 2. Connect your device to your PC via USB.
 3. On the computer, open a command prompt (on Windows) or terminal (on Linux or macOS) window inside the folder you installed adb & fastboot, and type:
```
adb devices
```
4. Your device should appear on the screen. Then to boot to fastboot type.
```
adb reboot bootloader
```
> [!Note]
> - You can also boot into fastboot mode via a key combination: turn the device off, hold Volume Up + Volume Down + Power.

5. Once the device is in fastboot mode, verify your PC finds it by typing:
```
fastboot devices
```
6. Type out the following command:
```
fastboot getvar all
```
- *Wait for a lot of text to finish scrolling and look for the “(bootloader) current-slot text”*
- *This should actually be toward the bottom without the need to scroll up*
- *The letter after this text will be the currently active partition slot (a or b) for your device*
        
7. Flash a recovery on your device by typing (replace <recovery_filename> with the actual filename!):
```
fastboot flash boot <recovery_filename>.img
```
8. Now change the active slot by typing (replace <slot> with the other slot that the previous command didn’t show.
> [!Warning]
> - For example if the previous command showed “(bootloader) current-slot a” you need to set b on <slot>):
```
fastboot --set-active=<slot>
```
9. Now use the menu to navigate (press on volume button) to and to select the Recovery option then press power button.
> [!Note]
> - If your recovery does not show the ProjectElixir logo, you accidentally booted into the wrong recovery. Please start again!

### Step 5: Flash Project Elixir ROM from recovery
1. Download the ProjectElixir zip package that you would like to install. 
2. If you are not in recovery, reboot into recovery:
3. With the device powered off, hold Volume Down + Power.
4. Now tap “Factory Reset”, then “Format data / factory reset” and continue with the formatting process (If it ask in what partition you want to format select “ext4”). This will remove encryption and delete all files stored in the internal storage, as well as format your cache partition (if you have one).
5. Return to the main menu.
6. Select “Apply Update”, then “Apply from ADB”.
7. On the PC open a terminal inside the adb & fastboot folder and sideload the package using (Replace <filename> with the actual filename!): 
```
adb sideload filename.zip
```
8. Wait until it finish.
9. Once you have installed everything successfully, click the back arrow in the top left of the screen,
10. Then “Reboot system now”

> [!Important]
> - If you get an errore like “adb sideload cannot read” download “Large Address Aware” (From this link: [Tap Here](https://www.techpowerup.com/forums/attachments/laa_2_0_4-zip.34392/) and open the executable.
> - On “Step 1: Select an executable” click on the "..." button to browse and select adb.exe from the folder you installed adb & fastboot.
> - Check the box on “Step 2: Large Address Aware Flag” to make it large address aware.
> - Click on Save
> - Then try sideloding & Wait ultil it finish

> [!Note]
> - Normally, adb will report Total xfer: 1.00x, but in some cases, even if the process succeeds the output will stop at 47% and report Total xfer: 0.98x or adb: failed to read command: Success. In some cases it will report adb: failed to read command: No error or adb: failed to read command: Undefined error: 0 which is also fine.
> - The first boot usually takes no longer than 15 minutes, depending on the device. If it takes longer, you may have missed a step, otherwise feel free to get assistance.
