# LLM Enabled Robot: Documentation

*Made: 09-19-2024*\
*Updated:09-20-2024*

## Software List:
Nvidia Jetson Orin: **Jetpack 5.1.2** with all appropiate Libraries (Cuda, etc)\
Zed Depth Camera Sensor: **ZED sdk 4.1** For Jetson Nano\
Elephat Robotics Cobot 280-M5-Stack: Download  Serial Driver, Firmware and PythonAPI. 

### Jetson Nano Orin Setup:
When getting a fresh Jetson Orin. 

Choose your Storage Media:
Micro-SD cards\
SSD N.vme (Preferred) 

Download List:

Make sure to download the correct version of Jetson Orin Jetpack (OS for Jetson line) on your computer **Jetpack 5.1.2**/

The reason for this is so it is compatible with ZED SDK, Robotic SDK, and ROS2 software. 

### Manual Setup: 
Use this if only Windows and MAC is all you have avalaible:

Go to this website for basic Setup Instructions:[Jetson Orin Setup](https://developer.nvidia.com/embedded/learn/get-started-jetson-orin-nano-devkit)

To also Image the OS to your file Storage download [balenaEtcher](https://etcher.balena.io/)

If more information is needed for firmware/install go to detailed [guide](https://www.jetson-ai-lab.com/initial_setup_jon.html)

### Automatic Setup: (NEED LINUX UBUNTU)
To Install OS, Software and Firmware easier use [NVIDIA SDK Manager](https://developer.nvidia.com/sdk-manager) (However can only be used with Ubuntu)

You could use a Virtual Machine that runs Ubuntu however this has restrictions when imaging, and most likely not work (I have tried) 

### Step 1 (Manual)

First Download the Operating System Image [here](https://developer.nvidia.com/embedded/jetpack-sdk-512)

<img width="1616" alt="Step_1_Download" src="https://github.com/user-attachments/assets/2b832d72-d5f8-4531-9f28-2db818b2e397">

### Step 2(Manual)
Then using [balenaEtcher](https://etcher.balena.io/)

Pick Flash from File

<img width="212" alt="Screenshot 2024-09-20 at 6 05 33 PM" src="https://github.com/user-attachments/assets/d0bf6e5f-0fc4-4c29-b6e4-f36aaa528cdd">

Select target which is your SD-Card that is inserted in your computer.

<img width="167" alt="Screenshot 2024-09-20 at 6 09 08 PM" src="https://github.com/user-attachments/assets/c7dc145f-c4f6-454e-a800-e1065e557199">


Then click Flash

<img width="161" alt="Screenshot 2024-09-20 at 6 09 36 PM" src="https://github.com/user-attachments/assets/8d495404-debd-43da-bd82-a29ef1fe66e9">



### Step 3 (Manual) 
Insert SD-Card to Jetson Board 

<img width="469" alt="Screenshot 2024-09-20 at 6 12 38 PM" src="https://github.com/user-attachments/assets/7aa1ceec-0ffb-4bf8-8377-6063f0d9b1dc">

Start the board, It should allow you to make your account after a long bootup process. (leave on for 10 minutes)

IMPORTANT if this step does not work after some time continue to the next steps

### Step 4 (Manual) Firmware:
If you SD-card does not start up it might be an issue with Firmware due to 5.1.2 being an older version it does not work with newer Firmware.

You must downgrade this Firmware to a lower version, Firmware version should be an Older UEFI version, and Nvidia l4t-core 35.4.1.

You can download all of this using this [link](https://developer.nvidia.com/embedded/jetson-linux-r3541) once downloaded you can upload this firmware using the onbaord UEFI. NOTE you need a USB drive for this or a direct connection to your laptop.

Once your Jetson Orin Nano boots up it will show you the UEFI screen. Click Tab

***Note: I Never Installed it in this way, I just saw online resources showing this as a way to downgrade***
***IF this firmware Install is proves too difficult please use the SDK Manager which I will show in the Automatic Section.***



Study Resources:\
[AI on the Jetson Nano LESSONS: Paul Mcwhorter](https://www.youtube.com/watch?v=5INy0FvaWLw&list=PLGs0VKk2DiYxP-ElZ7-QXIERFFPkOuP4_)

[Ultimate Jetson Orin Nano Walkthrough: Jetson Hacks](https://www.youtube.com/watch?v=qCAoPcMiR4k)






Arm Setup:



[Download Hub](https://www.elephantrobotics.com/en/downloads)


ZED Camera Setup:





Isaac-ROS2:










