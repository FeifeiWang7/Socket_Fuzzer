#### Download Source Code

from google git

#### Config Kernel

There are two approaches.

The first approach is to use the default config (suggested)

	ls arch/arm/configs/*exynos*
	
	ls arch/arm/configs/*manta*

	ARCH=arm make manta_defconfig

The second approach is to manually config

	ARCH=arm make menuconfig

#### Compile

Use cross compile

	make -j2 ARCH=arm CROSS_COMPILE=/home/feifei/Documents/android-ndk-r10e/toolchains/arm-linux-androideabi-4.8/prebuilt/linux-x86_64/bin/arm-linux-androideabi-

If success, there should be a zImage under arch/arm/boot directory

#### Boot

	adb reboot bootloader

	fastboot boot zImage
	
Check if boot successfully (according to timestamp)

	adb shell cat /proc/version
