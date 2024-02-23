![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Nothing Phone 1 (Spacewar)

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

### **Notes:-**
- If you are coming from A13 to A14 then clean flash is compulsory and format data.
- If you are encrypted do format Data before flashing build to avoid bugs.
- Rom is Encrypted

### Clean Flash :- 

### **Instructions:-**

---
**Step 1:**

First you need to [Unlock your bootloader](https://graph.org/How-to-unlock-bootloader-for-Nothing-Phone-1-07-15), skip to next step if you already.

---
**Step 2:**

> [!Important]
> If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options.

Download [Boot](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/recovery/boot.img/download) and [Vendor_boot](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/vendor/vendor_boot.img/download) from here and flash it through fastboot

```
---------------------------------------------
fastboot flash boot ./boot.img               |
---------------------------------------------
fastboot flash vendor_boot ./vendor_boot.img |
---------------------------------------------
```


---
**Step 3:**

After flashing above images, Reboot to Recovery.
```
fastboot reboot recovery
```
---
**Step 4:**

Factory reset > Format data/factory reset

Back to recovery home page & Apply update > Apply from ADB

Open command prompt & sideload rom using command adb sideload <rom_filename>.zip

---

### Dirty Flash :-
### **Instructions:-**

---
**Step 1:**

First you need to [Unlock your bootloader](https://graph.org/How-to-unlock-bootloader-for-Nothing-Phone-1-07-15), skip to next step if you already.

---
**Step 2:**

> [!Important]
> If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options.

Download [Boot](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/recovery/boot.img/download) and [Vendor_boot](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/vendor/vendor_boot.img/download) from here and flash it through fastboot

```
---------------------------------------------
fastboot flash boot ./boot.img               |
---------------------------------------------
fastboot flash vendor_boot ./vendor_boot.img |
---------------------------------------------
```

---
***Step 3:***

After flashing above images, Reboot to Recovery.
```
fastboot reboot recovery
```
---
**Step 4:**

Back to recovery home page & Apply update > Apply from ADB

Open command prompt & sideload rom using command adb sideload <rom_filename>.zip

---

> [!Note] 
> **Notes specific to device build**
> * Firmware and Gapps are already included in zip no need to flash additionally
> * If you are coming from Android 13 to Android 14 then clean flash is compulsory and format data.
> * If you are encrypted do format Data before flashing build to avoid bugs.

### **Enjoy [Project-Elixir](https://projectelixiros.com)**

<p align="center">
  <img src="https://i.imgur.com/uJQqd7q.png" />
</p>
