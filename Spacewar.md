<p align="center">
  <img src="https://i.imgur.com/gcOvt3T.png" />
</p>

# _Android 14(U) Installation Guide For Project-Elixir on Nothing Phone 1 (Spacewar)_

![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

`Note:- (Rom is Encrypted)`

## _Clean Flash_ :- 

### **Instructions:-**

---
***Step 1:*** 

_First you need to [Unlock your bootloader](https://graph.org/How-to-unlock-bootloader-for-Nothing-Phone-1-07-15), skip to next step if you already._

---
***Step 2:*** 

_Download [Boot](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/recovery/boot.img/download) and [Vendor_boot](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/vendor/vendor_boot.img/download) from here and flash it through fastboot_

```
---------------------------------------------
fastboot flash boot ./boot.img               |
---------------------------------------------
fastboot flash vendor_boot ./vendor_boot.img |
---------------------------------------------
```


---
***Step 3:***

_After flashing above images, Reboot to Recovery._
```
fastboot reboot recovery
```
---
***Step 4:***

_Factory reset > Format data/factory reset_

_Back to recovery home page & Apply update > Apply from ADB_

_Open command prompt & sideload rom using command adb sideload <rom_filename>.zip_

---

## _Dirty Flash_ :-
### **Instructions:-**

---
***Step 1:*** 

_First you need to [Unlock your bootloader](https://graph.org/How-to-unlock-bootloader-for-Nothing-Phone-1-07-15), skip to next step if you already._

---
***Step 2:*** 

_Download [Boot](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/recovery/boot.img/download) and [Vendor_boot](https://sourceforge.net/projects/project-elixir/files/fourteen/Spacewar/vendor/vendor_boot.img/download) from here and flash it through fastboot_

```
---------------------------------------------
fastboot flash boot ./boot.img               |
---------------------------------------------
fastboot flash vendor_boot ./vendor_boot.img |
---------------------------------------------
```

---
***Step 3:***

_After flashing above images, Reboot to Recovery._
```
fastboot reboot recovery
```
---
***Step 4:***

_Back to recovery home page & Apply update > Apply from ADB_

_Open command prompt & sideload rom using command adb sideload <rom_filename>.zip_

---

### **Notes:-**
- If you are coming from A13 to A14 then clean flash is compulsory and format data.
- If you are encrypted do format Data before flashing build to avoid bugs.

### _***Enjoy [Project-Elixir](https://projectelixiros.com)***_

<p align="center">
  <img src="https://i.imgur.com/uJQqd7q.png" />
</p>
