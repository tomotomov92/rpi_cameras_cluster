# Raspberry Pi Cameras Cluster
This is an example project on how to build **Raspberry Pi** with the following components:
- **Security Cameras Software**
- **VPN**
- **Network Storage**

The project has been made with the idea to create always powered on with low power consumption.
In order to accomplish this we're going to use Raspberry Pi 4 for server, Raspberry Pi Zero W for the cameras and open software which we can control and manage as we see fit.



## Equipment

### Recommended
> - **[Raspberry Pi 4](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/)** 2GB
> - **[Raspberry Pi 4 Type-C Power Supply](https://www.raspberrypi.org/products/type-c-power-supply/)** or comparable power supply poroviding at least 15W (5V 3A)
> - **[Raspberry Pi Zero W](https://www.raspberrypi.org/products/raspberry-pi-zero-w/)**
> - Power supply with Micro USB providing at least 5W (5V 1A)
> - **[Raspberry Pi Camera](https://www.raspberrypi.org/products/camera-module-v2/)** or **[Raspberry Pi Infrared Camera](https://www.raspberrypi.org/products/pi-noir-camera-v2/)**
> - SD Cards for each Raspberry Pi with at least 16GB storage

### Optional
> - [Case with heatsink](https://erelement.com/raspberry-pi-4/rpi4-al-case-black) for the Raspberry Pi 4
> - Waterproof case for the Raspberry Pi Zero W if it is going to be outside
> - [Heatsink](https://erelement.com/mini-pc/rpi-heat-sink) for the Raspberry Pi Zero W CPU
> - External Hard Drive for storing 



## Software

### Setting up Raspberry Pis
> - **[Raspberry Pi OS](https://www.raspberrypi.org/software/operating-systems/#raspberry-pi-os-32-bit)** for Raspberry Pi 4 - Preferebly Lite version
> - **[MotionEyeOS](https://github.com/ccrisan/motioneyeos/wiki/Supported-Devices#raspberry-pi-a-b-a-b-compute-module-zero-and-zero-w-models)** for Raspberry Pi Zero W
> - **[Raspberry Pi Imager](https://www.raspberrypi.org/software/)** for flashing the [Raspberry Pi OS](https://www.raspberrypi.org/software/operating-systems/#raspberry-pi-os-32-bit) and [MotionEyeOS](https://github.com/ccrisan/motioneyeos/wiki/Supported-Devices#raspberry-pi-a-b-a-b-compute-module-zero-and-zero-w-models) on the SD Cards. It is available for Windows, macOS and Ubuntu.



### Installations on Raspberry Pi 4

<details>
<summary>MotionEye</summary>

#### **[MotionEye](https://github.com/ccrisan/motioneye)** - The purpose of this software is to have centralized plase from where to manage the satelite cameras.
> - **[Install on Raspberry Pi OS](https://github.com/ccrisan/motioneye/wiki/Install-On-Raspbian)** 
> - **[Using Docker Image](https://github.com/ccrisan/motioneye/wiki/Install-In-Docker)** 

</details>


<details>
<summary>VPN</summary>

##### **[OpenVPN]()**
> - **[Install on Raspberry Pi OS](https://www.pivpn.io/)** 

##### **[WireGuard]()**
> - **[Install on Raspberry Pi OS](https://www.pivpn.io/)** 
> - **[Using Docker Image](https://hub.docker.com/r/linuxserver/wireguard)** 

</details>


<details>
<summary>Network Storage</summary>

##### **[Server Message Block](https://en.wikipedia.org/wiki/Server_Message_Block)**
> - **[Install on Raspberry Pi OS](https://pimylifeup.com/raspberry-pi-samba/)**

##### **[Network File System](https://en.wikipedia.org/wiki/Network_File_System)**
> - **[Install on Raspberry Pi OS](https://pimylifeup.com/raspberry-pi-nfs/)**

##### **[Apple Filing Protocol](https://en.wikipedia.org/wiki/Apple_Filing_Protocol)**
> - **[Install on Raspberry Pi OS](https://pimylifeup.com/raspberry-pi-afp/)**

</details>

## Install variants and how they look like

<details>
<summary>Install on Raspberry Pi OS</summary>



</details>

<details>
<summary>Using Docker Images</summary>



</details>