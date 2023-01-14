<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/211248683-9e2e62cf-cd80-4137-9861-f97980405faa.png" alt="Icono de GNS3">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/210186277-0d434bb0-80c0-43a9-b6b0-2e42e18c31a9.png" width="400" />
</p>

#  <img src="https://github.githubassets.com/images/icons/emoji/octocat.png" height="30" width="25" align="absmiddle"> GNS3 GUIDE <img src="https://github.githubassets.com/images/icons/emoji/octocat.png" height="30" width="25" align="absmiddle">


This is a repository of guides for installing GNS3 on different operating systems, as well as configuring devices and topologies. 

It can be helpful for beginners, self-learners or experts in the world of networking and virtualisation.

##  💡 What is GNS3?

- GNS3 is software used by hundreds of thousands of network engineers worldwide to emulate, configure, test and troubleshoot virtual and real networks. It allows you to run a small topology consisting of just a few devices on your laptop, to those who have many devices hosted on multiple servers or even hosted in the cloud.

- GNS3 is actively developed and supported, and has a growing community of over 800,000 members. By joining the community you will join other students, network engineers, architects and professionals who have downloaded it more than 10 million times to date. It is used in companies around the world, including Fortune 500 companies.

- GNS3 can help you prepare for certification exams such as Cisco CCNA, but it will also help you test and verify real-world implementations. Jeremy Grossman, the original developer of GNS3, created the software to help you study for your CCNP certifications. Thanks to that original work, today it can be used to help you do the same without paying for expensive equipment.

- GNS3 has enabled network engineers to virtualise real hardware devices for over 10 years. Originally only emulating Cisco devices using software called Dynamips, GNS3 has now evolved to support many devices from multiple network vendors, including Cisco virtual switches, Cisco ASA, Brocade vRouters, Cumulus Linux switches, Docker instances, HPE VSR, multiple Linux devices and many others. A list of devices supported by GN3 can be found at the following link: [Click](https://gns3.com/marketplace/appliances).

- GNS3 is not only compatible with Cisco devices. It is often discussed with Cisco because that is what most network engineers are interested in knowing. However, many other commercial and open source vendors support GNS3 today. You can now test interoperability between many vendors and even test esoteric configurations using networking technologies with SDN, NFV, Linux and Docker.

## ⚙ What is its architecture?

GNS3 consists of two software components:

- GNS3 All-in-One Software (GUI)
- GNS3 Server/Virtual Machine

## ✅ All-in-one GNS3 software

This is the graphical user interface (GUI) of GNS3 and the software part necessary for its operation. This package installs the all-in-one software on your local PC (Windows, MAC, Linux), so you can create your topologies using the included software. This is what you usually see in screenshots like the following:

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/Topologia-tipica-GNS3-696x378.png" width="400" />


## 📦 GNS3 Virtual Machine

When creating topologies in GNS3 you are using the graphical user interface (GUI), the created devices must be hosted and run by a virtual machine or server. You have a few options:

### 🟤 Local GNS3 server

It runs locally on the same PC where you installed the GNS3 all-in-one software. If, for example, you are using a Windows PC, both the GUI and the local server are running as Windows processes. Additional processes like Dynamips will also run on your PC.

### 🟣 GNS3 Virtual Machine

If you decide to use the GNS3 virtual machine (recommended), you can run the virtual machine locally on your PC using virtualisation software such as <a href="https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html" target="_blank">VMware Workstation</a> or <a href="https://www.virtualbox.org/wiki/Downloads" target="_blank">Virtualbox</a>; or you can run the GNS3 virtual machine remotely on a server using VMware ESXi or even in the cloud.

### 🟢 Emulation and Simulation in GNS3

GNS3 supports both simulated and emulated devices.

## 🟡 Emulation

GNS3 mimics or emulates the hardware of a device and runs real images on the virtual device. For example, you can copy the Cisco IOS from a real, physical Cisco router and run it on a virtual Cisco router emulated in GNS3.

## 🔴 Simulation

GNS3 simulates the functions and functionality of a device such as a switch. It is not running real operating systems, such as Cisco IOS, but rather a simulated device developed by GNS3, such as the GNS3 layer 2 switch.

### 🟣 Considerations between Simulation and Emulation in GNS3

The lines between simulation and emulation are blurring a bit these days. You can now run Cisco VIRL images which are images of real Cisco OS images running on standardised virtual hardware. GNS3 emulates the hardware that VIRL images require to run.

Don't worry too much about the difference between simulation and emulation, except for the following points:

- Dynamips is an older technology that emulates Cisco hardware. It uses real Cisco IOS images. It is good for basic CCNA type topologies, but has a number of limitations, such as only supporting older versions of Cisco IOS (12.X) which are also not supported or actively updated by Cisco.

- The recommended Cisco images to use are the Cisco VIRL images (IOSv, IOSvL2, IOS-XRv, ASAv). These images are supported and are actively updated by Cisco. The images support current Cisco IOS versions (15.X) and provide the best user experience and scale.


## 📦 Minimum, Recommended, Optimum Requirements

GNS3 is a platform that allows simulating network topologies with images from vendors such as Cisco and Juniper, among others. The requirements for installing the software are shown below.  

| Minimum Requirements | Recommended Requirements | Optimum Requirements |
| :--- | :--- | :--- |
| 2 GB RAM | 4 GB RAM | 8 GB RAM |
| 2 CPU Cores | 4 CPU Cores | 8 CPU Cores |
| 10 GB Free Disk Space | 20 GB Free Disk Space | 40 GB Free Disk Space |
| 1 Gbps Network | 1 Gbps Network | 1 Gbps Network |

```
Note: Virtualisation extensions are required. You may need to enable this through your computer's BIOS.
```

## 📌 Installation of GNS3 on Operating Systems

Go to the following path to learn how to install GNS3 on your operating system of choice: <a href="https://github.com/gherrada22/GNS3-Guide/tree/main/Installation%20of%20GNS3%20on%20Operating%20Systems" target="_blank">Here</a>.


## 📌 Image and Device Configuration

Go to the following step-by-step path to configure the GNS3 images and devices: <a href="https://github.com/gherrada22/GNS3-Guide/tree/main/Image%20and%20Device%20Configuration" target="_blank">Here</a>..


## ❤ How to support

- Giving the repository a star: If you like the project, please give it a star to help increase its visibility.

- Contributing to the project: If you want to contribute to the project, you can do it in the following ways:
  - By reporting bugs or errors.
  - By suggesting new features.
  - By translating the documentation into other languages.
  - By improving the documentation.

- Sharing the project: If you know someone who might be interested in the project, please share it with them.


## 🔰 NOTE

`This guide will be continuously updated (from basic to expert level). Greetings! :)`

&nbsp;

<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/210186277-0d434bb0-80c0-43a9-b6b0-2e42e18c31a9.png" width="400" />
</p>
</p>
<p align="center">Copyright &copy; 2023-present <a href="https://github.com/gherrada22" target="_blank">George Herrada Farfán</a>
