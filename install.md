
	ndk-build
	
	adb push socket-fuzzer /data/local/tmp

	adb shell
	
	cd /data/local/tmp

	./socket-fuzzer

	adb shell cat /proc/last_kmsg
