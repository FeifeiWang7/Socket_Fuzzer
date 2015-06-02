#### Setup Environment
Require
* JDK
* ADT Bundle for Mac (Eclipse, ADT plugin, Android SDK tools, Android Platforms-tool, Android platform)
* NDK

Configure

	vim ~/.bash_profile
        export PATH=${PATH}:/Users/feifei/Documents/adt-bundle-mac-x86_64-20131030/android-ndk-r9d
        export PATH=$PATH:/Users/feifei/Documents/adt-bundle-mac-x86_64-20131030/sdk/platform-tools
        export PATH=$PATH:/Users/feifei/Documents/adt-bundle-mac-x86_64-20131030/sdk/tools
	source ~/.bash_profile 

Test NDK
	
	cd /Users/feifei/Documents/adt-bundle-mac-x86_64-20131030/android-ndk-r9d/samples/hello-jni

	ndk-build
