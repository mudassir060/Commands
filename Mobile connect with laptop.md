# You need to connect to your device via adb connect:
adb connect <ip>:<port> 
# First you need to enable tcp mode as below with usb cable connected
# Plugin USB and execute
adb tcpip 5555
# Remove USB Cable and connect to your device via network:
adb connect <ip>:5555
# Now you can work with your device via network, enter shell as usual:
adb shell
# ⚠ WARNING: *Don't forget to DISCONNECT when you have finished debugging.
You can be in danger and may be listed at shodan.io and other sites similiar to shodan if you will keep tcpip be running in background. We can find your device via a simple portscan via masscan or similiar tools, so use below command when you are done in shell:

adb disconnect 
