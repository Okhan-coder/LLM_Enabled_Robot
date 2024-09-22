# **LLM-Enabled Robot: Documentation**

*Created: 09-19-2024*  
*Last Updated: 09-20-2024*

---

## **Table of Contents**
1. [Software List](#software-list)
2. [Jetson Nano Orin Setup](#jetson-nano-orin-setup)
   - [Choose Your Storage Media](#choose-your-storage-media)
   - [Manual Setup](#manual-setup)
     - [Step-by-Step Manual Setup](#step-by-step-manual-setup)
       - [Step 1: Download the OS Image](#step-1-download-the-os-image)
       - [Step 2: Using balenaEtcher](#step-2-using-balenaetcher)
       - [Step 3: Insert SD Card into Jetson Board](#step-3-insert-sd-card-into-jetson-board)
       - [Step 4: Firmware Downgrade](#step-4-firmware-downgrade)
   - [Automatic Setup (Linux Ubuntu)](#automatic-setup-linux-ubuntu)
3. [Study Resources](#study-resources)
4. [ZED Camera Setup](#zed-camera-setup)
5. [Cobot 280 Setup](#cobot-280-setup)
   - [Step 1: Hardware Setup](#step-1-hardware-setup)
6. [Isaac-ROS2](#isaac-ros2)
---

## **Software List**

- **Nvidia Jetson Orin**: *Jetpack 5.1.2* with all relevant libraries (e.g., CUDA)
- **ZED Depth Camera Sensor**: *ZED SDK 4.1* for Jetson Nano
- **Elephant Robotics Cobot 280-M5-Stack**: Download the Serial Driver, Firmware, and Python API

---

## **Jetson Nano Orin Setup**

### **Choose Your Storage Media**
- **Micro-SD card**
- **SSD NVMe** (*Recommended for optimal performance*)
> **Note:** Make sure you download the correct version of the Jetson Orin Jetpack OS on your computer: **Jetpack 5.1.2**.
### **Download the Necessary Files**



> This version is essential to ensure compatibility with ZED SDK, Robotics SDK, and ROS2 software.

## **Manual Setup**
If you're using Windows or Mac, follow these steps:
Software Needed:
- Visit the official setup page: [Jetson Orin Setup](https://developer.nvidia.com/embedded/learn/get-started-jetson-orin-nano-devkit)

To flash the OS image, use [balenaEtcher](https://etcher.balena.io/).

For a more detailed firmware/install guide, refer to this [Jetson Setup Guide](https://www.jetson-ai-lab.com/initial_setup_jon.html).
**Step-by-Step Manual Setup**

**Step 1: Download the OS Image**
Download the Jetpack 5.1.2 image from the official site [here](https://developer.nvidia.com/embedded/jetpack-sdk-512).

![Step 1 Download](https://github.com/user-attachments/assets/2b832d72-d5f8-4531-9f28-2db818b2e397)

**Step 2: Using balenaEtcher**
1. Launch [balenaEtcher](https://etcher.balena.io/).
2. Click on **Flash from File**.

   ![Flash from File](https://github.com/user-attachments/assets/d0bf6e5f-0fc4-4c29-b6e4-f36aaa528cdd)

3. Select your target SD card.

   ![Select Target](https://github.com/user-attachments/assets/c7dc145f-c4f6-454e-a800-e1065e557199)

4. Click **Flash**.

   ![Flash](https://github.com/user-attachments/assets/8d495404-debd-43da-bd82-a29ef1fe66e9)

**Step 3: Insert SD Card into Jetson Board**
- Insert the SD card into the Jetson board's slot.

![Insert SD Card](https://github.com/user-attachments/assets/7aa1ceec-0ffb-4bf8-8377-6063f0d9b1dc)

Power up the board. The setup process may take approximately 10 minutes. Follow the prompts to create your account.

> **Important:** If this step doesn’t work, continue to the next step.

**Step 4: Firmware Downgrade**
If the SD card doesn’t boot, there might be a firmware compatibility issue with Jetpack 5.1.2.

1. Download the older firmware from this [link](https://developer.nvidia.com/embedded/jetson-linux-r3541). You need an older UEFI version and Nvidia l4t-core 35.4.1.
2. Upload this firmware via the onboard UEFI using a USB drive or a direct connection to your laptop.

> **Note:** This method is based on online resources and has not been personally tested. If it’s too complex, use the SDK Manager.

---
**Automatic Setup (Linux Ubuntu)**
For a more streamlined installation process, use the [NVIDIA SDK Manager](https://developer.nvidia.com/sdk-manager).

> **Note:** The SDK Manager requires Ubuntu. You might attempt to use a virtual machine, but this method is often limited and might not work.

---



## **Study Resources**
- [AI on the Jetson Nano Lessons by Paul McWhorter](https://www.youtube.com/watch?v=5INy0FvaWLw&list=PLGs0VKk2DiYxP-ElZ7-QXIERFFPkOuP4_)
- [Ultimate Jetson Orin Nano Walkthrough by Jetson Hacks](https://www.youtube.com/watch?v=qCAoPcMiR4k)

---

## **ZED Camera Setup**
> **Details will be added soon**

---

## **Cobot 280 Setup**

### **Step 1: Hardware Setup**
1. Connect the power cable to the Cobot.
2. Use a USB-C cable or USB-to-USB cable to link it to your computer.

For downloads, visit the [Elephant Robotics Download Hub](https://www.elephantrobotics.com/en/downloads).

---

## **Isaac-ROS2**
> **Details will be added soon**

---










