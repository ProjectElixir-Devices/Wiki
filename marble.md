![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Poco F5 / Redmi Note 12T (Marble)

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
   - **Recovery Link**: [Tap here to download](https://www.pling.com/p/2131814/)

3. Download the Project Elixir ROM for Poco F5 / Redmi Note 12T from a reliable source.
   - **Project Elixir ROM Link**: [DOWNLOAD](https://projectelixiros.com/device/marble/)


### How To Flash Recovery
```
- Download Recovery From link Below
- Open platform Tools Folder in pc/laptop
- Open Command Prompt 
- fastboot flash recovery_ab recoveryimagename.img 
- congrats Recovery is flashed 
- Now reboot to Recovery and follow further steps
```

### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Boot to Recovery - must use A14 recovery - link below
- Wipe Dalvik/Cache + Metadata
- Flash your regional latest Firmware (Link Below)
- Flash the Rom
- Reflash the recovery or You can simply tick on Flash current recovery while flashing
- Format Data
- Reboot to system
```

### Dirty Flashing Steps
```
- Wipe dalvik cache
- Flash the ROM (Update of the same ROM!)
- Flash current recovery (You can tick on flash current recovery)
- Clean cache (Not necessary)
- Reboot to System
```

> [!Important]
> - A14 recovery: [Tap here for link](https://www.pling.com/p/2131814/)
> - Firmware : [Tap Here for link](https://t.me/chaitanyabuilds/52705)
> - If facing Sms bug toggle sim on off on every boot and for rooted users flash this [smsfix zip file](https://sourceforge.net/projects/project-elixir/files/fourteen/marble/smsfix/)
>    * If u r not receiving OTP or sms after booting rom or after restart, flash this in ksu or magisk and allow mobile to reboot
Or
If u r not rooted, u can Toggle sim off and on once. If still doesn't fix, then turn sim off first, then restart ur Mobile and then turn sim on.
> - Flash [This](https://github.com/tiann/KernelSU/releases/download/v0.7.6/AnyKernel3-android12-5.10.198_2023-11.zip) if Ksu Required

> [!Note] 
> - ROM comes with Gapps inbuilt no need to flash gapps.
> - If you are coming from Android 12 or 13 to Android 14 then clean flash is compulsory.
> - Melt Kernel is not Supported
> - First Boot time may take 2 minutes so wait
> - Reboot time may be 30 seconds for some cases approx
> - Wait For atleat 1 day for the rom to settle down
