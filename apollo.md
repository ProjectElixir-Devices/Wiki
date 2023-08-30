![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For Project Elixir on Redmi K30S Ultra/Mi 10T/Pro (apollo)




**Start with unlocked bootloader and grab a PC with windows, linux or macOS**



**Req:**
```
Download platform-tools and extract it
Download ROM + recovery.img and place files in platform-tools folder
then connect your phone to PC.
```

1. Open CMD, and navigate to your platform-tools folder. Then fastboot boot recovery:
```
fastboot boot recovery.img
```
2. On device, navigate to "Apply Update" & select "Apply from ADB"
3. On PC, sideload the ROM (copy paste the zip name)
```
adb sideload "ROM-name".zip
```
***Wait for it to complete.***

4. On device, navigate back to home screen (top left arrow) and find "Factory Reset"
```
This will factory reset the device, removing all user data
```
5. Boot and enjoy - firmware and recovery are included with the ROM

<br>
<br>

**Dirty flashing:***
```
Just adb sideload the zip and reboot, that's all!
```

**Note:**
- IF YOU ARE MOVING FROM ANOTHER ROM, CLEAN FLASH Is COMPULSORY.
- If adb sideload fails, unplug and replug the device to PC and try again
- GCamGO included
