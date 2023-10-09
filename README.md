# Esp32Cam
Esp32Cam with ability to reconfigure Wifi network in real time and on demand.

This was modified from example CameraWebServer with help from [WifiManager library](https://github.com/tzapu/WiFiManager) and its examples.

  After reboot, if there is no saved Wifi connection, it will set up a portal at 192.168.4.1 via CamWifiConfigure hotspot so that we can configure Wifi. If we want to use another Wifi network, just press and hold trigger button in about 10s (second), then it will enter configuration mode and set up that portal again.
  
  Spare GPIO13 pin was used as trigger button since most of other pins were occupied by other tasks. Moreover it was easy to connect to external button with less hassle, like below figure:
  
   ![Esp32-Cam-MB with button](https://github.com/hanhha/Esp32Cam/assets/2361076/9c53a1ce-f4b6-44a1-a5c4-975472393346)
  
  I just used a normal push button, stripped 2 pins and used pliers to straighthen remaining 2 pins, then pushed them into the header of Esp32Cam-MB module before stacking Esp32Cam module. Then bended the button and adhered it to the header by super glue. It was easy to make it fit in a case. 
  

