### First you need to enable tcp mode as below with usb cable connected
### Plugin USB and execute
    adb tcpip 5555
### Remove USB Cable and connect to your device via network:
    adb connect "IP":5555
    .\adb devices
### Check list of devices attached:
    adb devices
### Now you can work with your device via network, enter shell as usual:
    adb shell
### ⚠ WARNING: *Don't forget to DISCONNECT when you have finished debugging.
You can be in danger and may be listed at shodan.io and other sites similiar to shodan if you will keep tcpip be running in background. We can find your device via a simple portscan via masscan or similiar tools, so use below command when you are done in shell:
    adb disconnect 

### Adb Server
    adb kill-server
    adb start-server 

### App install with apk file
    adb -e install path/to/app.apk

-d                        - directs command to the only connected USB device...
-e                        - directs command to the only running emulator...
-s <serial number>        ...
-p <product name or path> ...
The flag you decide to use has to come before the actual adb command:

adb devices | tail -n +2 | cut -sf 1 | xargs -IX adb -s X install -r com.myAppPackage // Install the given app on all connected devices.

### Uninstalling app from device
    adb uninstall com.myAppPackage
    adb uninstall <app .apk name>
    adb uninstall -k <app .apk name> -> "Uninstall .apk withour deleting data"