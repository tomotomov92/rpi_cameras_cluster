# RPi0 W Installation


### I: Download MotionEyeOS for Raspberry Pi and install Flashing software

1. Download the [MotionEyeOS](https://github.com/ccrisan/motioneyeos/wiki/Supported-Devices#raspberry-pi-a-b-a-b-compute-module-zero-and-zero-w-models) version for [Raspberry Pi 0](https://github.com/ccrisan/motioneyeos/releases/download/20200606/motioneyeos-raspberrypi-20200606.img.xz)

2. Connect the Raspberry Pi 0 Camera cable to the Raspberry Pi 0 and the camera
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/1.2.png)

3. Prepare `wpa_supplicant.conf` file for connecting to the wireless network
```
country=BG
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1

network={
    ssid="WiFiName"
    psk="WiFiPassword"
}
```


### II. Flash image on SD Card

1. Open Raspberry Pi Imager

2. Load MotionEyeOS
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/2.2.1.png)
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/2.2.2.png)
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/2.2.3.png)

3. Select SD Card
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/2.3.1.png)
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/2.3.2.png)

4. Flash the image to the SD Card
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/2.4.1.png)
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/2.4.2.png)
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/2.4.3.png)

5. Copy `wpa_supplicant.conf` to boot drive

6. Eject SD Card from 


### III: Configure system settings

1. Log-in into the RPi 0 W from the web browser
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/3.1.png)
```
Username: admin
Password:
```

2. Update **General Settings** password
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/3.2.png)

3. Update **General Settings** Time Zone
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/3.3.png)

4. Update **General Settings** Hostname
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/3.4.png)

5. Update **Expert Settings** Overclocking to `turbo`
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/3.5.png)

6. Update **Expert Settings** Enable System Monitoring to `ON`
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/3.6.png)

7. Apply changes


### IV: Configure Camera details

1. Update **Video Device** Camera Name
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/4.1.png)

2. Update **Video Device** Video Resolution to `1000x1000`
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/4.2.png)

3. Update **Video Device** Frame Rate to `15`
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/4.3.png)

4. Update **Video Streaming** Streaming Quality to `50%`
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/4.4.png)

5. Apply changes


### V: Configure external storage

1. Update **File Storage** Storage Device to `Network Share`
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/5.1.png)

2. Update **File Storage** Network Server to the IP of the IF of RPi4-Server
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/5.2.png)

3. Update **File Storage** Share Name
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/5.3.png)

4. Update **File Storage** Root Directory to `/`
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/5.4.png)

5. Test Share
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/5.5.1.png)
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/5.5.2.png)

6. Apply changes


### VI: Configure recordings and motion detection

1. Update **Movies** Movie File Name
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/6.1.png)

2. Update **Motion Detection** Frame Change Threshold to `1.5%`
![](https://raw.githubusercontent.com/tomotomov92/rpi_cameras_cluster/main/images/RPi0/6.2.png)

3. Apply changes