# Sierra-Wireless-EM74xx-Series-WWAN-Card-Driver-for-macOS-Catalina

These drivers work for Sierra Wireless EM7455/EM7430 Qualcomm Snapdragon X7 LTE-A WWAN cards under macOS 10.15.6 Catalina. 

To make these cards working under macOS 10.15.6, you only need proper USB Mapping and open their two ports: COM6 and COM8. 

To modify this kext in order to drive the cards under other 10.15.x versions:
1. Find the build number of the OS at "About this Mac -- Version 10.15.x". Hover the cursor at the line for a second, then the 5-digit build number will appear. 
2. Copy them, open "/Legacy_Sierra_QMI.kext/Contents/Info.plist", change "BuildMachineOSBuild" to your build number. 
3. Save, load and then restart. You will find information about the card displayed correctly both at the "WWAN" slot and "USB" slot in SystemInformation.app, and the signal sign will appear on the status bar. 

