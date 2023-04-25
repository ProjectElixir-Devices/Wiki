![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For Project Elixir on Munch

•Reboot device into fastboot mode.
[Press vol down (-) and power button]

• Download the boot.img & vendor_boot.img from the website.

• Install adb-system wide or use platform tools. 

• Connect the device via a cable then type the following commands in the command prompt window:-

### Command :

```
fastboot flash boot [boot.img location] && fastboot flash vendor_boot [vendor_boot.img location] && fastboot reboot recovery
```

• Now your device will boot into the PE recovery, Now-

• Do a factory reset if CLEAN flashing

OR

• Directly proceed to adb sideload if DIRTY flashing.

• To start Sideloading select the apply update option and sideload the file, command is:-

### Command :

```
adb sideload [ROM.zip location]
```

### Alternate Flashing Method

• You can also use TWRP or OFOX recovery for flashing Elixir.


### Elixir Boot & Vendor Boot Image Download 

https://mega.nz/folder/z3BlWYzA#VkrcjpQJM5Q0KweHaFi8Yg


### NOTE:-
• Firmware is built-in ( indian users to flash indian fw )

• GAPPS are built-in

• Clean Flash is compulsory if coming from any version of MIUI or any other custom ROM, dirty flash works if updating from an older Elixir build of the same Android version and is by the same maintainer.
