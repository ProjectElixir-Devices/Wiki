![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide For Project Elixir on MI 11 Pro

-Enter fastboot

-Flash boot.img

Code:

fastboot flash boot_ab boot.img

-Boot to recovery (can do from bootloader or with buttons from power off state)

-Now in recovery go to factory reset and confirm the reset

-Reboot to recovery

-Choose apply update and Apply from ADB

-Now install Elixir zip via sideload

Code:

adb sideload Elixir.zip

-Go back to main menu and reboot


Update installation:

-Via recovery:

Boot to recovery

Choose apply update and Apply from ADB

Now install Elixir zip via sideload and reboot

Code:

adb sideload Elixir.zip

If you had gapps, reboot to recovery and sideload gapps.zip and reboot


-Via OTA:

Go to Settings -> System -> Updater and download latest build

Choose install and let it finishIf you have Magisk installed, don't click reboot when prompted and go to Magisk and choose install to inactive slot

Reboot

### Note: 
No need to flash the firmware separately, it is built-in

No need to flash the gapps separately, it is built-in
