![Installation Guide For Project Elixir on Mojito](https://i.imgur.com/Hb3gl9Q.jpg "Installation")

# Installation Guide For Project Elixir on Mojito/Sunny

## IF YOU ARE MOVING FROM ANDROID 10 or ANDROID 11 TO ANDROID 12 then CLEAN FLASH ( Format Data ) Is COMPULSORY.


Now let's continue , here are the steps.

## A. with PE recovery

1. boot to pe recovery (command is fastboot flash boot pe_rec.img)

2. format data (factory reset)

3. Now Go To Pc,Open CMD In Platform Tools,Type adb sideload rom_file.zip(File Name Will Be Different)

It Will Be Failed At 47%.It's Normal So Dont Worry.

Now Reboot Your Phone And Enjoy!



## B. with TWRP 

1. boot to twrp ( command is fastboot boot twrp.img)( then go to advanced > install ramdisk twrp.img / flash currrent twrp )

2. with twrp there's 2 ways to use it , either using adb sideload with pc or prepare rom file in sdcard / otg pendrive.

3. Now for direct flash is assuming u have rom files in sdcard /otg pendrive , first choose in twrp menu wipe > format data > type yes ( dont worry if internal storage is zero , it's normal , u have to boot to rom first to able to access it , which is why recommended having rom files in a sdcard / otg pendrive) ( noted if u using sideload with twrp dont need to worry bout anything)

4. now after formatting data , reboot recovery once and start flashing your rom (ignore any red line mounted error , just pay attention to top left corner of twrp if it written successful , u good to go) and wait for process . 

5. after flashing is successful , go to advanced > install ramdisk / flash current twrp to kept the twrp (noted this step need to be done everytimes right after flashing a rom if u don't want to lose the twrp) 

6. now reboot to system ( magisk.zip can be flashed after boot to rom ) and enjoy your rom 

7. make sure to enable either lockscreen password or pole before booting to twrp again to temporarily decrypt phone for rom flashing (just type your lockscreen pass) .
