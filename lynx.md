<p align="center">
  <img src="https://github.com/Project-Elixir/docs/blob/bkl/res/elixir-a16banner.png" />
</p>

### Introducing Project Elixir now based on Android 16 シ
> <p>"Redefine Simplicity with your android experience on our minimalistic custom rom — where sleek design meets robust security, performance, and stability."</p>

### ⊀ Unleash Innovation ⊁

> Elevate your user interface with minimalist design and with the striking of perfect balanced customization options, customize with ease.

### Installation Guide for Pixel 7a (lynx)

> [!CAUTION]
> - Your warranty is void. Or valid, probably?
> - Project Elixir is not responsible for any damage you made to your device. You have been warned!
> - Don't fall for mod/cracks etc and you may end up in trouble, in such scenarios you are not to blame us.

> [!Warning]
> * We are not responsible for anything that may happen to your phone by installing custom ROMs.
> * We are not responsible for anything that may happen to your phone by installing any kernels.
> * You do it at your own risk and take the responsibility upon yourself
> * You are not to blame Project Elixir or its respected developers for any of your loss.
> * Be careful while going through download, installation guide, changelog links as A12 = v2.0 (snow), A13 = v3.0 (Tiramisu) and A14 = v4.0 (UNO), A15 = 5.0 (vany) and A16 = v6.0 (bkl) respective branch.

> [!Tip]
> **Basic Notes for all users:**  
> * The provided instructions are for Project Elixir based on Android 16.
> * These will only work if you follow every section and step precisely
> * Do not continue after something fails! Contact in support group for help
> * The device must have an unlocked bootloader & has Platform Tools installed in pc.
> * If you are moving from any other Android version to Android 16, it is necessary to do CLEAN FLASH (Format Data)
> * Take a backup for safe side (If you are coming from older Android version or doing a clean flash)
> * For any queries or help related to Elixir, join our support group : [Tap Here](https://telegram.me/Elixir_Discussion)  

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Project Elixir ROM for from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/lynx)

3. Download the Recovery/Boot/other required files:
   - **Reqired files Link [ For Android 16 ]:** [Tap Here](https://projectelixiros.com/device/lynx)

> [!Warning]
> * I am assuing that you have already unlocked the bootloader and ready to go. If not then please unlock your bootloader first using fastboot mode.
> * If you are unsure what firmware version you are currently on, we strongly recommend returning to the corresponding stock OS before following the installation guide!
> * Unlocking the bootloader will erase all data on your device! Before proceeding, ensure the data you would like to retain is backed up to your PC and/or your Google account, or equivalent.
> * Please note that OEM backup solutions like Samsung and Motorola backup may not be accessible from Project Elixir once installed.

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
> [!Important]
> - If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options
7. Now, reboot your device into Fastboot Mode using the following command:
```
adb -d reboot bootloader
```

### Step 3: Unlock Bootloader using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:
```
fastboot devices
```
> [!Note] 
> If your device is listed, you are ready and If you don’t get any output or an error:
> * **On Windows:** Download [latest fastboot driver](https://xdaforums.com/t/official-tool-windows-adb-fastboot-and-drivers-15-seconds-adb-installer-v1-4-3.2588979/) and copy the folder into your desktop, then go again in Device Manager, locate your device, right-click on your device and choose "Update driver", choose "Browse my computer for driver software", then “Browse…” and select the folder you copied in your desktop. Click “ok” and then on “next”.
> * **on Linux or macOS:** If you see no permissions fastboot try running fastboot as root. When the output is empty, check your USB cable and port!
2. Now type the following command to unlock the bootloader:
```
fastboot flashing unlock
```
> [!Tip] 
> * At this point the device may display on-screen prompts which will require interaction to continue the process of unlocking the bootloader.
> * Give next/agree to actions the device when it asks you to proceed.
3. If the device doesn’t automatically reboot, reboot it. It should now be unlocked.
4. Since the device resets completely, you will need to re-enable USB debugging to continue.

### Step 4: Boot it into Fastboot/Bootloader mode
~ This platform requires additional partitions to be flashed for recovery to work properly, the process to do so is described below.
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:
```
fastboot devices
```
2. If your device is listed, you are ready to proceed. Download the required files from the link provided in Step 1.
> * boot.img
> * dtbo.img
> * vendor_kernel_boot.img
3. Place the downloaded files in the same location as the platform-tools folder on your computer.
4. Now, flash them by using the following command one by one:
```
fastboot flash boot boot.img
```
```
fastboot flash dtbo dtbo.img
```
```
fastboot flash vendor_kernel_boot vendor_kernel_boot.img
```
5. Once done then move forward to next step i.e. **Step 5**

### Step 5: Installing Elixir Recovery using fastboot

1. Download Elixir Recovery. Simply download the latest recovery file named **vendor_boot.img** from the link provided in Step 1.
> [!Tip]
> - *Replace `recovery_file_name.img` with the actual name of the Elixir Recovery image you downloaded if needed*
> - *Other recoveries may not work for installation or updates. We strongly recommend to use the one we provide*
> - *Some devices have buggy USB support while in bootloader mode, if you see fastboot hanging with no output when using commands such as fastboot getvar ..., fastboot boot ..., fastboot flash ... you may want to try a different USB port (preferably a USB Type-A 2.0 one) or a USB hub*

2. Flash recovery onto your device:
```
fastboot flash vendor_boot vendor_boot.img
```
3. Now reboot into recovery to verify the installation.
4. Use the menu to navigate to and to select the Recovery option.
5. Your device will reboot with Elixir Recovery installed.
> ***If your recovery does not show the Elixir logo, then you accidentally booted into the wrong recovery. Please start at the top of this section (Step 4)!***

### Step 6: Installing Project Elixir from recovery
1. Download the Project Elixir zip file that you would like to install
2. If you are not in recovery, reboot into recovery
3. Now tap Factory Reset, then Format data / factory reset and continue with the formatting process.
> [!Warning]
> *This will remove encryption and delete all files stored in the internal storage, as well as format your cache partition (if you have one)*
4. Return to the main menu and start sideloading the zip/package (On the device, select “Apply Update”, then “Apply from ADB” to begin sideload.)
>   *but do not reboot before you read/followed the rest of the instructions* 
6. Open command prompt & sideload rom using command 
```
adb -d sideload filename.zip
```
3. Once you have installed everything successfully, you can now reboot your device into the OS for the first time!
4. Click the back arrow in the top left of the screen, then “Reboot system now”.

> [!Tip]
> - The first boot usually takes no longer than 15 minutes, depending on the device. If it takes longer, you may have missed a step
> - After the package is installed, recovery will inform you that reboot to recovery is required to install add-ons. In that case please select “NO,” as we ship Gapps by deafult.
> - Normally, adb will report Total xfer: 1.00x, but in some cases, even if the process succeeds the output will stop at 47% and report adb: failed to read command: Success.
> - In some cases it will report adb: failed to read command: No error or adb: failed to read command: Undefined error: 0 which is also fine.

### Enjoy Project Elixir
> - Congratulations! You've successfully installed Project Elixir on your device
> - Enjoy the new features and customization options that the ROM offers
> - Remember, if you encounter any issues during the installation process, feel free to seek help from the Project Elixir community or refer to their official documentation.

> [!Note] 
> **Notes specific to device build**
> * Gapps is already included in zip no need to flash additionally
> * First boot usually takes no longer than 15 minutes, depending on the device. If it takes longer, you may have missed a step.
> * If you are coming from PORTs then you need to Format Data and flash latest firmware [depending on the device]
> * If you are coming from Android 12/13/14/15 to Android 16 then clean flash is compulsory and format data.
> * If you are encrypted do format Data before flashing build to avoid bugs.

<br>

> [!Tip]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)

<p align="center">
  <img src="https://github.com/Project-Elixir/docs/blob/bkl/res/elixir-copyright.png" />
</p>
