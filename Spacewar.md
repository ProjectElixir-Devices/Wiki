![Installation Guide For Project Elixir](https://i.imgur.com/42LxtAl.png)

### Installation Guide For Project Elixir on Nothing Phone 1 (Spacewar)

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



### **Enjoy [Project-Elixir](https://projectelixiros.com)**

<p align="center">
  <img src="https://i.imgur.com/uJQqd7q.png" />
</p>
