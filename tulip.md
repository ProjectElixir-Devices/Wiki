![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Redmi Note 6 Pro (tulip)

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
### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Boot to recovery - Wipe cache,dalvik,system,data,vendor
- Format data
- Flash retrofit dynamic supported TWRP - must use recommended recovery - link below
- Wipe dalvik/art,cache,data
- ( untick the option of unmount system before flashing from TWRP settings )
- Flash the latest build
- Format Data
- Reboot to system
```

### Dirty Flash
```
- Download the latest build
- Boot to recovery - Wipe dalvik/art,cache,data
- Flash the latest build
- Reboot to system
```

> [!Important]
> **Required Files:**
> * Retrofit Dynamic Recovery: [Tap here for link](https://sourceforge.net/projects/mocha-development/files/tulip/twrp/dynamic.recovery.img/download)

> [!Note]
> **Notes specific to device build**
> * Gapps are already included in zip no need to flash additionally.
> * We have Switched Retrofit Dynamic Partitions from v4.1 or above
> * If you are coming from A13 to A14 clean flash is compulsory and format data.
