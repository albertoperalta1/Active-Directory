# Basic Home Lab Running Active Directory

This repository contains steps on how i set up a basic home lab running Active Directory following a tutorial by [Josh Madakor](https://www.youtube.com/@JoshMadakor)

## Diagram
![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/e9c3fe97-1215-4243-88e4-175dec5f7131)

## Download and install Oracle VirtualBox from the official website.
[Oracle Virtual Box](https://www.virtualbox.org/)

## Download the Windows 10 and Server 2019 ISO files.
[Windows 10 iso](https://www.microsoft.com/en-us/software-download/windows10ISO)
[Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

## Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media.

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/b39d0f0b-ebd5-43c0-b3fe-f3b41548b4e7)

<img width="672" alt="Screenshot 2024-04-15 at 8 45 34 AM" src="https://github.com/albertoperalta1/Active-Directory/assets/166507731/9f997792-4fcd-472d-81da-6b72461b5578">

##  Configure the virtual machine by giving it two network adapters: one for connecting to the internet and the other for the private network.

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/8080ccff-7b79-4d02-aae2-6b850b79902f)

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/38961832-456a-4f87-9234-9acf3c1c45eb)

##  Install Server 2019 on the virtual machine and assign IP addressing for the internal network.

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/cd5e0cea-1c36-471e-b80c-bc613995fd40)

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/67156555-85cc-4a05-bf4c-b401f8e83101)

##  Name the server and install Active Directory to create the domain.
![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/92672b42-b3b5-41f0-9b54-c5c11a8057ba)

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/7aadf375-a790-449d-a759-6a3ca614a289)

##  Configure routing so that clients on the private network can access the internet through the domain controller.
![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/054f2fdb-2a35-4bd0-bafb-be62469a8614)

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/c512e083-c4e2-4c5d-9a2b-2a75e2d977c4)

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/9d3ab94e-ad6b-412b-a07d-733719c42229)

##  Set up DHCP on the domain controller.
![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/43b3a4b2-ecdf-4c33-8fa8-04e309e4b4c3)

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/a64bc90e-0451-4fdd-b1e4-a62b3c3dae6b)

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/a6b7bd4a-e60e-4069-af70-6636ce26bc84)


##  Run the PowerShell script to create 1000 users in Active Directory.

[Power Shell script for creating users](https://github.com/joshmadakor1/AD_PS)

##  Create a new virtual machine named "Client1" and install Windows 10 on it

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/764348c1-1557-4d90-9c08-77451b27d651)


##  Connect the client machine to the private network and join it to the domain.
<img width="859" alt="Screenshot 2024-04-15 at 9 17 42 AM" src="https://github.com/albertoperalta1/Active-Directory/assets/166507731/e1b24f3c-84d8-4930-a728-b4e62c948f37">

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/051e27b9-103a-4ad2-8c9e-3915c89f6268)



##  Log into the client machine with a domain account.

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/a3d46085-5c7c-4b04-914d-8d61921a26d3)

![image](https://github.com/albertoperalta1/Active-Directory/assets/166507731/a0a69d77-69a9-4885-aec9-3afede4e0bf7)
