<p align="center">
  <img src="https://i.imgur.com/irnHU8d.png" />
</p>

### Introducing Project Elixir now based on Android 15 シ
> <p>"Redefine Simplicity with your android experience on our minimalistic custom rom — where sleek design meets robust security, performance, and stability."</p>

### ⊀ Unleash Innovation ⊁

> Elevate your user interface with minimalist design and with the striking of perfect balanced customization options, customize with ease.

### Installation Guide for Project Elixir on Generic System Image (gsi)

> [!CAUTION]
> - Your warranty is void. Or valid, probably?
> - Project Elixir is not responsible for any damage you made to your device. You have been warned!
> - Don't fall for mod/cracks etc and you may end up in trouble, in such scenarios you are not to blame us.

> [!Warning]
> * We are not responsible for anything that may happen to your phone by installing custom ROMs.
> * We are not responsible for anything that may happen to your phone by installing any kernels.
> * You do it at your own risk and take the responsibility upon yourself
> * You are not to blame Project Elixir or its respected developers for any of your loss.
> * Be careful while going through download, installation guide, changelog links as A12 = v2.0 (snow), A13 = v3.0 (Tiramisu) and A14 = v4.0 (UNO) and A15 = 5.0 (vany) respective branch.

> [!Tip]
> **Basic Notes for all users:**  
> * The provided instructions are for Project Elixir based on Android 15.
> * These will only work if you follow every section and step precisely
> * Do not continue after something fails! Contact in support group for help
> * The device must have an unlocked bootloader & has Platform Tools installed in pc.
> * If you are moving from any other Android version to Android 15, it is necessary to do CLEAN FLASH (Format Data)
> * Take a backup for safe side (If you are coming from older Android version or doing a clean flash)
> * For any queries or help related to Elixir, join our support group : [Tap Here](https://telegram.me/Elixir_Discussion)  

> [!Important]
> **PREREQUISITES:**
> - Check Project treble compatibility using [Treble Info](https://play.google.com/store/apps/details?id=tk.hack5.treblecheck)
> - Must have A/B partitioning or System-As-Root support
> - Must fit into ARM64 architecture requirement. (Future builds may include A64 support)
> - Must have at least VNDK28 support.



1. Get [Platform Tools](https://developer.android.com/studio/releases/platform-tools#downloads)
2. Get vbmeta.img from Stock ROM or [Google](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img)
4. Get Elixir GSI
5. Boot into bootloader mode:
```
adb reboot bootloader
```
6.Flash the vbmeta you got from step two
```
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
```
7. Boot into fastbootd
```
fastboot reboot fastboot
```
8. Flash GSI
```
fastboot flash system GSI-FILENAME.img
```

> [!Warning]
> * If fastboot tells you there isn't enough place, you can try to delete product/system_ext partitions.
> * I recommend flash an empty image on thems to avoid problems with magisk.
> * Download File : [placebo](https://drive.google.com/file/d/1HqW-9zE2VgUI2KQcae2F4-82wOyL0HbP/view?usp=sharing)
```
fastboot flash product placebo.img
```
```
fastboot flash system_ext placebo.img
```
9. And try to flash GSI again
10. Go back to recovery, then perform "Factory reset / Wipe data"
11. Reboot and enjoy :D

> [!Warning]
> **MEDIATEK DEVICES AND CERTAIN EXYNOS MAY NOT BOOT**

> [!Important]
> * For SAMSUNG DEVICES
> * Vbmeta must be flashed trough Odin/Heimdall and isn't required to boot for some devices.
> * Requires patched recovery to access fastbootd: [Patch](https://github.com/Johx22/Patch-Recovery)
> * Flash it through Odin/Heimdall.
> * Boot it and select enter fastboot (fastbootd)

<br>

> [!Note] 
> **Notes specific to device build**
> * Gapps is already included in zip no need to flash additionally
> * If you are coming from Android 12 or 13 to Android 14 then clean flash is compulsory and format data.
> * If you are encrypted do format Data before flashing build to avoid bugs.

<br>

> [!Tip]
> **Donate**: [Do consider donating or buying us a coffee](https://projectelixiros.com/donate)

<p align="center">
  <img src="https://i.imgur.com/bETSPlo.png" />
</p>
