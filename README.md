# Motorola Moto e 2020

## Rooting
Download the latest APK for Magisk: https://github.com/topjohnwu/Magisk/releases

Also download the appropriate ROM for the phone from [here](#images)

TWRP and OrangeFox do not work with motorola-ginna currently.

1. Install the Magisk APK.
2. Using the ROM you downloaded, extract `boot.img`.
3. Move the `boot.img` to your phone.
4. Inside of Magisk, "Install" > "Install" > "Select and Patch a File". Select the boot.img you moved to the phone and transfer the patched file back to the computer.
5. Boot the phone into fastboot mode by holding the Volume Down and Power buttons. 
6. Ensure your device shows up in `fastboot devices`. 
7. Run `fastboot flash boot_a patched_boot.img` and `fastboot flash boot_b patched_boot.img`. Note that the second (`boot_b`) might not run, don't worry about that.
8. `fastboot reboot` and ensure Magisk says the device is rooted.

## Images
http://motostockrom.com/

- Note that you only need the "Firmware" directory from the motostockrom image.
- You'll want to have this website on hand to recover the device if flashing it goes wrong.

## PostmarketOS
Work needs to be done to port ginna to PostmarketOS. This repository should help with that. See the `APKBUILD` and `deviceinfo` files. Both are heavily based on the MSM8916 mainlining guide.

## Resources
- https://github.com/ixmoe/android_device_motorola_ginna_twrp
- https://github.com/ixmoe/android_kernel_motorola_sdm632
- https://github.com/msm8953-mainline/linux
- https://wiki.postmarketos.org/wiki/Qualcomm_Snapdragon_450/625/626/632_(MSM8953)
- https://wiki.postmarketos.org/wiki/MSM8916_Mainlining
- https://wiki.postmarketos.org/wiki/Porting_to_a_new_device#Device_specific_package
motorola-ocean might be similar enough to grab stuff from that.
