A complete HOWTO by PTX64 ( https://forum.xda-developers.com/m/ptx64.11988819/ ) for unlocking and installing a secure, Google-less, LineageOS 19.1 on the Redmi Note 10 (mojito), including the latest Xiaomi firmware, TWRP + FBE-Disabler, Magisk + modules (for MicroG, Safenet, SSH), AuroraStore, Google Camera, AdAway and AFWall.

Eventually you'll end up with a fully Google Authenticated, Google-less, fast, lightweight and hardened device, which allows you to use most app's on it. But it will also block internet access to newly installed/rogue apps, (Google) app spying habits, bloatware, advertisements and more by default.

*All copyright goes the respected owners, everything you do is at your own risk. Installing and using the Xiaomi unlock, fastboot and ADB tools is only covered in simple command terms because this is out-of-scope of this HOWTO.

*You'll need Windows for the Mi Unlock App, though using the app under Wine or QEMU in Linux might be possible. Most Linux distributions provide the required USB driver by default, and you can install ADB and fastboot though the package manager. For Windows, you'll need to install the lastest ADB/fastboot tool from here https://androidmtk.com/download-minimal-adb-and-fastboot-tool , and the last mentioned driver here if Windows update cannot find one on his own trough Windows update and/or when you uninstall the Mi Unlock App: https://gsmusbdriver.com/xiaomi-mi-note-10



## 1. Unlocking the device. (If you don't or didn't do this properly, you'll will end up with issues or a bricked device later on).

- First ensure your official MIUI OS is up to date, backup your phone and do a factory reset on it.

- Then follow this guide: https://c.mi.com/thread-2262302-1-0.html , grow a beard in the meantime and complain to Xiaomi. And yes, the excuses for the locking device in this manner has mostly to due with revenue, control and monitoring by Xiaomi, not mainly user security.


* When the device is now unlocked:

- Go to “Settings” > “Mi Account” > “Mi Cloud”.

- Turn off all synchronization options and most importantly disable “Device Search”.

- At this point the verification should start and phone number will be requested (otherwise you can enter Mi account ID number or email).

- Next enter your account password, fill in captcha and device search will be disabled.

- Go back to “Mi Account” and press “Quit Mi Account”, you’ll see 3 available options, select “Delete from phone”.


## 2. Updating and clean reflashing the device. (Again, if you don't do this, you'll will end up with issues or a bricked device later on).

This step is to ensure you have a fully up-to-date and clean device. You can repeat this step too if you want to revert back to your official Xiaomi MIUI personal spy device and re-lock the device afterwards.

- Unsure that the correct USB driver, fastboot and ADB tools are installed.

- Download and extract the latest firmware here: https://bigota.d.miui.com/V13.0.9.0.SKGMIXM/mojito_global_images_V13.0.9.0.SKGMIXM_20220616.0000.00_12.0_global_2e8598ffa6.tgz

- Power off the device. Hold "volume down" + "power" button until the fastboot logo appears.

- Connect your USB-C cable to your phone and computer.

- The command "fastboot devices" should now show a serial-number > fastboot is working.
- Go to the map of the extracted firmware, and run "flash_all.bat" or "flash_all.sh" under Linux. Check for error's and if everything is OK, the phone will reboot when done.


## 3. Installing the firmware Blob, LineageOS, TWRP and Magisk.
Working on it...
