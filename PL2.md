![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Nokia 6.1 (PL2)

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

### Unlocking the Bootloader [1/4] :

> [!Note] 
> The steps below only need to be run once per device.


> [!Warning]
> Unlocking the bootloader will erase all data on your device! Before proceeding, ensure the data you would like to retain is backed up to your PC and/or your Google account, or equivalent.

 1. Install Nokia USB Drivers (required): To ensure that your device is properly detected during the bootloader unlock process, make sure to install the required. If you already have the required drivers installed you can skip this step. To install the drivers, download [this](https://github.com/StollD/nokia-driver-installer/blob/master/out/Phone_Nokia_USB_Driver_v1.4.0.exe) installer package from GitHub and install it to your computer.
 
 2. Download and extract the Nokia Bootloader Unlock tool from [here](https://tchms.to/NokiaUBLTool). Using this tool you can easily unlock the bootloader of your device without touching the command line. Use a zip management tool of your choice to extract the tool to a folder on your computer.

> [!Note]
> The tool currently only supports Windows 7 or later with Microsoft .Net Framework version 4.7.2 or higher. Linux or Mac are not supported. Windows 10 with latest updates is recommended

 1. Reboot the phone into download mode: Now you need to boot your device to download mode. Follow these steps for bootloader mode:
 
  - Turn off your phone.
  - Connect the USB cable to the device only and not the computer.
Press and hold Volume Down + Power key together till you reach the screen reads that reads “Download mode”.
  - Press and hold Volume Down + Power key together till you reach the screen reads that reads “Download mode”. Alternatively, you can also use the command `adb reboot bootloader` from the stock ROM to bring the phone to download mode.
 
 2. Generate OTP for the Unlock Tool: To avoid misuse and limit usage, the tool uses OTP (One-time password). Before you unlock you need to get an OTP. You can generate one from [here](https://www.techmesto.com/nokia-ubl-otp/)

> [!Note]
> The OTP is valid for only 15 minutes from generation. In addition only 15 devices are allowed for unlocking each day. After this further generation of OTPs will be disabled for the day. If the OTP generation fails, please be patient and wait for the next day to try again

 1. Run the Unlock Tool and unlock your phone Now you can use the previously generated OTP to unlock the bootloader of your device.

   - Run the “Bootloader Unlock by tm.exe” file in the folder where you extracted the tool
   - Paste the OTP (from step 3) into the Enter OTP box in the Unlock Tool.
   - Connect your smartphone in download mode.
   - Click on the “BEGIN UNLOCK” button.
   - Wait for the process to complete and follow the instructions shown in the output window.
   - Your device should prompt you for unlock. Use the volume keys to accept the unlock.
 2. Once the device bootloader unlocked follow up with the next steps.

### Ensuring all firmware partitions are consistent [2/4 - Optional] :

> [!Note]
> The steps below only need to be run once per device.

 1. Download the latest firmware from [Here](https://sourceforge.net/projects/fihsw-sdm660/files/PL2/FIHSW_PL2-415C-0-00WW-B01_600WW_10_20200501.full.lzma2.8196b83ea498b17a172bbb95f46b94cb3bab32404f2493a818e390f858a55eaf.7z/download)
 2. Download the `HCTSW Care OSTRemote Client tool` & follow the usage/flashing guide from [Here](https://xdaforums.com/t/tools-hctsw-care-ostremote-client-batch-script-replacement-of-ost-la.4282019/).
 3. Once the firmware installation is done, now power off the device & follow up the below steps.
Retrofit 

### Retrofit Dynamic Partititions instruction [3/4] :

> [!Warning]
> Retrofit Dynamic partition must be initialized when installing for the first time, so the process to do so is described below.

 1. Reboot your device into `Download mode/fastboot mode`
 2. Install the `Nokia Driver` from [Here](https://github.com/StollD/nokia-driver-installer/raw/master/out/Phone_Nokia_USB_Driver_v1.4.0.exe)
 3. Download `Platform tool` by Google from [Here](https://developer.android.com/tools/releases/platform-tools)
 4. Download the `super_empty.img` from [Here](https://github.com/ProjectElixir-Devices/device_nokia_PL2/releases/download/PL2-RDP/super_empty.img)
 5. Now flash `super_empty.img` file with the given command `fastboot wipe-super <PATH TO Super-empty.img>`
 6. Now follow up with the below steps.

### ROM installation [4/4] :

 1. Reboot your device into `fastboot mode/Download mode`
 2. Type `fastboot device`, if the device S/N detected then everything is all good. [If not detected install the [Nokia Driver](https://github.com/StollD/nokia-driver-installer/raw/master/out/Phone_Nokia_USB_Driver_v1.4.0.exe) & [Platform tool](https://developer.android.com/tools/releases/platform-tools)]
 3. Now flash the boot.img (ProjectElixir recovery) in both the slots by the following commands:
 
```
fastboot flash boot_a <PATH_TO_boot.img>
fastboot flash boot_b <PATH_TO_boot.img>
```
 4. Now reboot into `recovery mode` by holding the Volume Up & Power button.
 5. Apply Update » adb sideload method & sideload the ProjectElixir .zip file by `adb sideload <PATH_TO_ProjectElixir4.x-*.zip>`
 6. Once the installation done, perform the `Factory reset` then » `Reboot to system`

### Installing Project Elixir from recovery:

 1. Download the [ProjectElixir installation package](https://projectelixiros.com/device/PL2) that you would like to install.
 2. If you are not in recovery, reboot into recovery:
With the device powered off, hold `Volume Up` and connect to a computer.
 3. Now tap Wipe.
 4. Now tap Format Data and continue with the formatting process. This will remove encryption and delete all files stored in the internal storage.
 5. Sideload the ProjectElixir `.zip` package:
  - On the device, select “Advanced”, “ADB Sideload”, then swipe to begin sideload.
  - On the host machine, sideload the package using: `adb sideload filename.zip.`

> [!Tip]
> Normally, adb will report `Total xfer: 1.00x`, but in some cases, even if the process succeeds the output will stop at 47% and report `Total xfer: 0.98x` or `adb: failed to read command: Success`. In some cases it will report `adb: failed to read command: No error` or `adb: failed to read command: Undefined error: 0` which is also fine.

 6. Once you have installed everything successfully, run ‘adb reboot’.

> [!Note]
> The first boot usually takes no longer than 15 minutes, depending on the device. If it takes longer, you may have missed a step, otherwise feel free to get assistance.

> [!Warning]
> Depending on which recovery you use, you may be prompted to install additional apps and services. We strongly advise you to opt out of installing these, as they may cause your device to bootloop, as well as attempt to access or corrupt your data.

> [!Tip]
> If the installation process reports the message "(~47%) adb: failed to read the command: No error", do not worry, the process was completed successfully and you can restart the device.

> [!Important]
> Donate: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)
