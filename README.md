# MSI-B450m-MORTAR-Hackintosh
MSI-B450m-MORTAR-MAX-Hackintosh

## Description
macos: sonoma 14.0 (23A344)

opencore: 9.5  
motherboard: MSI-B450m-MORTAR-MAX  
cpu: AMD Ryzen 5 5600   
gpu: AMD Radeon RX 6600 XT  
audio: usb audio (due to bad of motherboard)  
disk: nvme J.ZAO   
usb: USB port has been customized   
wifi：intel AX210 （works properly with driver preview.05）   
bluetooth: intel and it works fine   

## Bios setting
disable security boot  
csm -> uefi  
disable Serial port  
**disable above 4G**  （sleep issue related）  

## Attention
- customized your own usb port,  built-in ports maybe different 

- remove my own built-in disk 

- gen your own platformInfo 

- ## Highlights


1. Rename cpu name: AMD Ryzen 5 5600 6-Core Processor

2. AMD CPU sensor :  [AMDRyzenCPUPowerManagement.kext](OC/Kexts/AMDRyzenCPUPowerManagement.kext)  [SMCAMDProcessor.kext](OC/Kexts/SMCAMDProcessor.kext) 

3. AMD GPU sensor:  [SMCRadeonGPU.kext](OC/Kexts/SMCRadeonGPU.kext)  [RadeonSensor.kext](OC/Kexts/RadeonSensor.kext) 

4.  Radeon 6600

   ```xml
<key>@0,name</key>
<string>ATY,Henbury</string>
<key>@1,name</key>
<string>ATY,Henbury</string>
<key>@2,name</key>
<string>ATY,Henbury</string>
<key>@3,name</key>
<string>ATY,Henbury</string>
<key>ATY,DeviceName</key>
<string>W6600X</string>
<key>ATY,EFIVersion</key>
<string>01.01.270</string>
<key>ATY,FamilyName</key>
<string>Radeon Pro</string>
<key>device_type</key>
<string>ATY,HenburyParent</string>
<key>model</key>
<string>AMD Radeon Pro W6600X</string>
<key>name</key>
<string>ATY,Henbury</string>   
   ```


## Preview
<img src="https://github.com/MagicianLjj/MSI-B450m-MORTAR-Hackintosh/blob/main/ScreenShot/about.png" width="196"/>
<img src="https://github.com/MagicianLjj/MSI-B450m-MORTAR-Hackintosh/blob/main/ScreenShot/sensei.png" width="556"/>

## Acknowledgements 
国光：https://apple.sqlsec.com/6-%E5%AE%9E%E7%94%A8%E5%A7%BF%E5%8A%BF/6-1.html  
黑果小兵：https://blog.daliansky.net/   
corpnewt: https://github.com/corpnewt/CPU-Name  

