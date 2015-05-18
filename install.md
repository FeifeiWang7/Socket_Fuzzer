#### Setup Environment
Require
* JDK
* ADT bundle (eclipse with SDK and adt)
* NDK

For Mac, just download the .dmg, double click, and click continue to finish the installation of JDK.

Configure NDK
	vim ~/.bash_profile
	export PATH=${PATH}:/Users/feifei/Applications/adt-bundle-mac-x86_64/android-ndk-r9d
	source ~/.bash_profile 

Test NDK
	ndk-build
