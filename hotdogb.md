![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For Project Elixir on hotdogb

- When Bootloader is already unlocked
- Download [recovery from here](https://download.lineageos.org/devices/hotdogb/builds) for lineage-20.0-20230618-nightly-hotdogb-signed.zip 
### Note: Recovery for newer build does not work

- Download latest Project Elixir Hotdogb build
- Boot into fastboot
```
fastboot flash recovery recovery.img
```
- Boot into recovery
- Do Factory reset if coming from from different ROM
```
adb sideload ProjectElixir_3.*_hotdogb-13.0-20230627-1927-OFFICIAL.zip
```
### Note: Use the latest zip name when sideloading

- There will be prompted that it fail security validation check, press yes to install
- Reboot

