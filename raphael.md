![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

## Installation Guide For Project Elixir on Raphael

#### Clean Flash
```

1. flash ofox fbev1 recovery (decrypted user's can use official ofox).
2. wipe dalvik, cache, system, vendor, data.
3. flash A11 FW (according to your device region).
4. flash ROM.
5. flash dfe (if decrypted user).
6. format data (decrypted user's can skip this).
7. reboot to system.
8. enjoy.
```

#### Dirty Flash
```

1. flash rom.
2. flash dfe (if decrypted user).
3. flash magisk (if previously you were using).
4. wipe dalvik, cache.
5. reboot to system.
6. enjoy.
```

#### Temporary ScreenOffFod Fix
```

Root method :
1. install termux from play store
2. give su permission
3. run this command "su -c settings put secure screen_off_udfps_enabled 1"
4. to disable it run this command "su -c settings put secure screen_off_udfps_enabled 0"


ADB method:
1. connect your phone to PC/Laptop
2. run this command "adb shell settings put secure screen_off_udfps_enabled 1"
3. to disable it run this command "adb shell settings put secure screen_off_udfps_enabled 0"
```
