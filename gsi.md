![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on GSI Device

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


### MEDIATEK DEVICES AND CERTAIN EXYNOS MAY NOT BOOT AT THIS TIME

> [!Important]
> **PREREQUISITES:**
> - Check Project treble compatibility using [Treble Info](https://play.google.com/store/apps/details?id=tk.hack5.treblecheck)
> - Must have A/B partitioning or System-As-Root support
> - Must fit into ARM64 architecture requirement. (Future builds may include A64 support)
> - Must have at least VNDK28 support.

CLEAN FLASH:
```
- Download GSI system image
- Extract .xz file
- Boot into recovery
- Flash extracted system.img file as 'System'
- Wipe Cache, Dalvik and format Data
- Reboot system
```

DIRTY FLASH:
```
- Download GSI system image
- Extract .xz file
- Boot into recovery
- Wipe dalvik, cache
- Flash the system.img file as 'System'
- Reboot To System
```

<br>

> [!Note] 
> **Notes specific to device build**
> * Gapps is already included in zip no need to flash additionally
> * If you are coming from Android 12 or 13 to Android 14 then clean flash is compulsory and format data.
> * If you are encrypted do format Data before flashing build to avoid bugs.

<br>

> [!Important]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)
