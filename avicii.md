MUST KNOW SHIT(Necessary for first timers, not for repeaters.If this is not your first time trying a custom rom and you dont know these shit. Better stop trying any custom rom)
	1)Backup everthing before doing anything (Swift Backup recommended, needs rooted phone tho)
	2)Remove Screen lock security
	3)Install Adb drivers, qualcomm drivers and fastboot drivers in PC
	4)Download Platform Tools
	5)Run CMD in PLatform Tools Directory
	6)Finsih up Fastboot installations
	7)OEM unlock, Bootloader unlock
		Turn on developer settings
`		Turn on OEM unlock, USB debugging
		Reboot to FASTBOOT
		Run command
			fastboot devices
			fastboot flashing unlock
		Use volume buttons to navigate and Unlock Bootloader
		It will wipe your data and reboot your system. 
	5)Do offline setup. 
	6)Turn on Developer options
	7)Turn on USB debugging
	8)Run "adb devices" on CMD in PlatformTools Directory and authorise the device
	9)Necessary things DONE!!!!

INSTALLING THE ROM
	1)Reboot to Bootloader
	2)Download AOSP Recovery or PEX Recovery(stable version of your Device and Android version respectfully and place them in PlatformTools Diretory)
	3)Run command
		fastboot devices
		fastboot boot (Any recovery name).img
 	4)It will boot into the recovery image
	5)Tap on Update, update from ADB sideload
	6)Download and custom ROM zip file and place it in the PlatformTools Diretory
	7)Run Command
		adb sideload (Name of the Rom).zip
	8)If it fails, tap on advanced, reboot to bootloader and try the other recovery
	9)The installation takes upto 10 mins, and fails exactly at 47%
	10)Factory reset in the recovery image
	11)Reboot to System
	12)Hopefully you're all set with a new ROM of your choice

Sayonara Bois!!!