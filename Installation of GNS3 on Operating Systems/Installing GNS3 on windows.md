<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/211248683-9e2e62cf-cd80-4137-9861-f97980405faa.png" alt="Icono de GNS3">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/210186277-0d434bb0-80c0-43a9-b6b0-2e42e18c31a9.png" width="400" />
</p>

# 🔰 Download GNS3

Download the software from its official repository <a href="https://www.gns3.com/software/download" target="_blank">here</a>.


## 🟡 Starting the GNS3 installation on windows 

1. Once the download is finished you must run the file, then you will be asked for administrator permissions, give Ok and the following screen will appear as the image, this refers to the license agreement to run the installation GNS3. Click on `I Agree`.

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-5.png" width="400" />

2. Then choose the Folder where the shortcut will be installed in the start menu (See Image), it is recommended to leave it as default.

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-6.png" width="400" />

3. **Selection of components for the GNS3 installation.**

You will then be asked to select the components to be installed along with GNS3, as shown in the table. Please note which components are included during the installation of GNS3, as well as the function of each component and their developers' website. It is recommended that all components be selected and installed.


| Component | Description | Developer |
| --- | --- | --- |
| GNS3 | GNS3 is a graphical network simulator that allows you to design complex network topologies. | [GNS3](https://www.gns3.com/) |
| WinCap | WinPcap is a packet capture library for Windows. | [WinPcap](https://www.winpcap.org/) |
| WireShark | Wireshark is a network protocol analyzer. | [Wireshark](https://www.wireshark.org/) |
| Dynamips | Dynamips is a Cisco router emulator. | [GNS3](https://rednectar.net/tag/dynamips/) |
| QEMU | QEMU is a generic and open source machine emulator and virtualizer. | [QEMU](https://www.qemu.org/) |
| VPCS | VPCS is a virtual PC emulator. | [GNS3](https://sourceforge.net/projects/vpcs/) |
| Cpulimit | Cpulimit is a tool to limit the CPU usage of other processes. | [Cpulimit](	http://cpulimit.sourceforge.net/) |
| TightNVC Viewer | TightNVC Viewer is a remote desktop viewer. | [TightNVC](https://www.tightvnc.com/) |
| SolarWinds | SolarWinds is a network management software. | [SolarWinds](https://www.solarwinds.com/) |
| Response Time Viewer | Response Time Viewer is a network management software. | [Response Time Viewer](https://www.solarwinds.com/) |
| Npcap | Npcap is a packet capture library for Windows. | [Npcap](https://nmap.org/npcap/) |

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-7.png" width="400" />

3.1. Next, select the folder where the application will be installed, in this case the default folder has been left as shown in the image.

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-8.png" width="400" />

4. Then the file copy is started as shown in the picture. Additional applications such as Visual C++ will be installed, give you the accesses so that the application can run smoothly. 

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-9.png" width="400" />

4.1. In some cases an internet connection will be required to download applications such as Wireshark.

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-10.png" width="400" />

5. Then the copy of the files is completed as shown in the image. Click Next to continue.

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-11.png" width="400" />

6. Then I will see a screen asking to install the Solarwinds Standard Toolset application, it is an application that helps in the administration, management and monitoring of networks, if you need it you can install it, this is the link to the application so you can consult more information: [Here](https://www.solarwinds.com/es/engineers-toolset).

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-12.png" width="400" />

7. Finally, the GNS3 installation is completed. Select Start GNS3.

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/image-13.png" width="400" />

8. First Start: GNS3 Setup Wizard

After installation, the next step is to configure the graphical user interface using the Setup Wizard, in order to host the IOS images, this can be done using a virtual machine or server, the image. It shows the screen at the first start of GNS3.

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/04/selecci%C3%B3n-del-servidor-para-la-simulaci%C3%B3n-en-gns3.png" width="400" />


9. GNS3 Local Server Configuration

In the Setup Wizard choose "Run only legacy IOS on my computer" and click Next, then choose the location where the application "gns3server.exe" is located, as well as the IP and port. It is recommended to set the following parameters:

- `Server path:` Default location of the executable gns3server.EXE.
- `Host Binding:` Set IP 127.0.0.1 which is the loopback IP address.
- `Port:` 3080 TCP.

<p align="center">
  <img src="https://www.telectronika.com/wp-content/uploads/2018/05/image3.png" width="400" />


## 📌 Additional note

- `Run Modern IOS (IOSv or IOU), ASA and appliances from non Cisco manufacturers:` Requires configuration of a Virtual Machine.
- `Run only legacy IOS on my computer:` IOS loading can be done directly on the GNS3 platform via local server.
- `Run everything on a remote server (for advanced users):` loading of devices is done through remote servers.

&nbsp;

<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/210186277-0d434bb0-80c0-43a9-b6b0-2e42e18c31a9.png" width="400" />
</p>
</p>
<p align="center">Copyright &copy; 2023-present <a href="https://github.com/gherrada22" target="_blank">George Herrada Farfán</a>