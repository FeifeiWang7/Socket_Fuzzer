#### Setup Environment
Require
* JDK
* ADT Bundle for Mac (Eclipse, ADT plugin, Android SDK tools, Android Platforms-tool, Android platform)
* NDK

For JDK, use java6. Open eclipse, there will be a prompt for quick install of java6.

Configure NDK

	vim ~/.bash_profile

	export PATH=${PATH}:/Users/feifei/Documents/adt-bundle-mac-x86_64-20131030/android-ndk-r9d
	export PATH=$PATH:/Users/feifei/Documents/adt-bundle-mac-x86_64-20131030/sdk/platform-tools
	export PATH=$PATH:/Users/feifei/Documents/adt-bundle-mac-x86_64-20131030/sdk/tools

	source ~/.bash_profile 

Test NDK

	cd /Users/feifei/Documents/adt-bundle-mac-x86_64-20131030/android-ndk-r9d/samples/hello-jni	

	ndk-build

Open Eclipse, install subversion

	brew search subversion

Choose version 1.7.x

	brew install --universal --with-java homebrew/versions/subversion17

	sudo mkdir -p /Library/Java/Extensions

	sudo ln -s /usr/local/lib/libsvnjavahl-1.dylib /Library/Java/Extensions/libsvnjavahl-1.dylib
