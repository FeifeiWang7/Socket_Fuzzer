#### Setup Environment
Require
* JDK
* ADT Bundle for Mac (Eclipse, ADT plugin, Android SDK tools, Android Platforms-tool, Android platform)
* NDK

For Mac, just download the .dmg, double click, and click continue to finish the installation of JDK.

Configure NDK

	vim ~/.bash_profile

	export PATH=${PATH}:/Users/feifei/Applications/adt-bundle-mac-x86_64/android-ndk-r9d

	source ~/.bash_profile 

Test NDK
	
	cd /Users/feifei/Applications/adt-bundle-mac-x86_64/android-ndk-r9d/samples/hello-jni

	ndk-build
