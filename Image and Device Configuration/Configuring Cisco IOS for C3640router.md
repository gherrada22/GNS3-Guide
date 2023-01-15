<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/211248683-9e2e62cf-cd80-4137-9861-f97980405faa.png" alt="Icono de GNS3">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/210186277-0d434bb0-80c0-43a9-b6b0-2e42e18c31a9.png" width="400" />
</p>

## 🔱 Configuring Cisco IOS for C3640 router.

- If you are a network engineer you must know the most famous network simulator GNS3. From here you can download the Cisco C3640 series IOS for GNS3. But before I give you the download link, I want to discuss some features and advantages of GNS3 over the other network simulators.

- GNS3 is a graphical network simulator where you can create and build simple and complex network scenarios on your computer virtually. In this way, you test your configuration before implementing it in the real network. You can use different network devices with GNS3 such as routers, virtual PC, cloud, etc. [Here for more information](https://github.com/gherrada22/GNS3-Guide)


- The 3640 Router Simulation Appliance in GNS3 is an intermediate-level router model that is used in small and medium-sized enterprise networks and in CCNA and CCNP study labs. It is based on MIPS processor architecture hardware, and features a variety of network interfaces, including Ethernet, Token Ring, and serial.

- The c3640-ik9o3s-mz.124-25b.image is a specific version of IOS for this device, with a release date of 25 September 2005. This version includes all the IOS features and functionalities mentioned above, such as dynamic routing, access control, network services, and management and monitoring tools.

- In addition, this version of IOS supports a variety of dynamic routing protocols, including OSPF, EIGRP, BGP, and RIP, allowing users to configure and simulate a variety of network scenarios. It also includes a number of security features, such as packet filtering and authentication, allowing users to simulate a secure network environment.

- In summary, c3640-ik9o3s-mz.124-25b.image is an IOS image for a 3640 router simulation device on GNS3, with a variety of features and functionality, including dynamic routing, access control, network services, and management and monitoring tools, that allows users to configure and simulate a variety of network scenarios and prepare for Cisco certifications. [Here is the link for GNS3 Switch IOS](https://github.com/gherrada22/GNS3-Guide/tree/main/Image%20and%20Device%20Configuration/Download%20%20IOS%20Cisco).

## 🟤 Features

- Support for network protocols such as TCP/IP, IPX/SPX, AppleTalk, and many others.

- Dynamic routing using protocols such as OSPF, EIGRP, BGP and RIP.

- Network access control through security policies and packet filtering.

- Connectivity features, such as VPN and WAN link.

- Network services such as DHCP, DNS, and NTP.

- Management and monitoring tools to help network administrators monitor and troubleshoot network problems.


```
Note: Please note that this IOS image is for GNS3 use only. For commercial use, you must purchase it from your nearest Cisco.com or Cisco partner in your local region.
```

## ✅ Import Image in GNS3

In the GNS3 GUI, click `Edit > Preferences` to open the Preferences menu.

<p align="center">
  <img src="https://i.ibb.co/Lk05R88/gns3.jpg" width="400" />

In the preferences menu, select `IOS Routers and New`, to begin the process of importing an image.

<p align="center">
  <img src="https://docs.gns3.com/img/getting-started/setup-wizard-local-server/9.jpg" width="400" />

You will be asked which server you want to run the image on, but everything except `Run IOS router on my local computer` should be greyed out.

<p align="center">
  <img src="https://docs.gns3.com/img/getting-started/setup-wizard-local-server/10.jpg" width="400" />

On the next screen, click `Browse` to import a compatible IOS image:

<p align="center">
  <img src="https://docs.gns3.com/img/getting-started/setup-wizard-local-server/11.jpg" width="400" />

Go to the folder where you have stored your Cisco IOS images, select the image and click `Open`:

<p align="center">
  <img src="https://i.ibb.co/YZ6Pb67/gns31.jpg" width="400" />

GNS3 can decompress IOS images to allow faster start-up of routers in your GNS3 topologies. This is recommended for a better user experience. Click `Yes` to decompress the image:

<p align="center">
  <img src="https://i.ibb.co/TR4t5Dd/iso.jpg" width="400" />

```
⚠ Important:
==============================================================================================================================================================
- By selecting "No", the compressed IOS Image will be kept, then, when the router is switched on at initialisation, the decompression process will be performed.
==============================================================================================================================================================
- Otherwise, if "Yes" is selected, the image will be decompressed, the loading will be much faster and the above described process of decompression during initialisation will not occur.
==============================================================================================================================================================
```

The directory where the uncompressed image is stored is displayed. Click `Next` to continue with the configuration:

<p align="center">
  <img src="https://i.ibb.co/1QrSLmZ/iso2.jpg" width="400" />

The **Name and Platform** window appears. Confirm the platform selection and configure the router name. Active `This is an EhterSwitch router` and click `Next`:

<p align="center">
  <img src="https://i.ibb.co/1LWQRpR/iso4.jpg" width="400" />


```
- The "This is an EtherSwitch router" option in the IOS file of a Cisco 3640 device is used to enable the switch functions on the device. This allows the device to function as an Ethernet switch instead of a traditional router.

- When this option is enabled, the device can perform switching tasks, such as learning MAC addresses and routing traffic based on the MAC address. Additional features are also enabled, such as support for VLANs and the ability to configure ports in trunk or access mode.
```

<p align="center">
  <img src="https://i.ibb.co/9rzLzmD/etherswitch.jpg" width="400" />

A default RAM configuration is displayed. It is important that you check the minimum memory requirements of your router using the Cisco website. Click on the `Check minimum and maximum RAM requirement` option:


<p align="center">
  <img src="https://docs.gns3.com/img/getting-started/setup-wizard-local-server/16.jpg" width="400" />

Cisco Feature Navigator opens in your default web browser. Select Image Name and enter the name of the image you are using:


<p align="center">
  <img src="https://docs.gns3.com/img/getting-started/setup-wizard-local-server/17.jpg" width="400" />


Set the default RAM value to the value recommended by Cisco Feature Navigator (yours may be different from the screenshot) and click `Next`:


<p align="center">
  <img src="https://docs.gns3.com/img/getting-started/setup-wizard-local-server/20.jpg" width="400" />

Select your preferred network adapters. This depends on the device.

```
Know the functionalities of each card. Below is a summary of the functionality of each interface.
```

| Interface | Function | Number of Ports |
| :--- | :--- | :--- |
| [PA-A1](https://www.cisco.com/c/en/us/td/docs/interfaces_modules/port_adapters/install_upgrade/atm/pa-a1_ATM_install_config/a1_0c3sm/3455over.html) | ATM network interface | 1xATM |
| [PA-FE-TX](https://www.cisco.com/c/en/us/td/docs/interfaces_modules/port_adapters/install_upgrade/ethernet/pa-fe_100baset_fast_ethernet_install_config/2659v2fe/2899over.html) | Fast Ethernet network interface | 	1xFE (10Mb) |
| [PA-2FE-TX](https://www.cisco.com/c/en/us/td/docs/interfaces_modules/port_adapters/install_upgrade/ethernet/pa-2fe_tx-fx_install_config/pa_2fetx/3474ovr.html) | Dual Fast Ethernet network interface | 2xFE (10Mb) |
| [PA-GE](https://www.cisco.com/c/en/us/td/docs/interfaces_modules/port_adapters/install_upgrade/ethernet/pa-ge_gigabit_ethernet_install_config/pa_ge/2696over.html) | Gigabit Ethernet network interface | 1xGE (1000Mb) |
| [PA-4T+](https://www.cisco.com/c/en/us/td/docs/interfaces_modules/port_adapters/install_upgrade/serial/pa-4t-_sync_serial_install_config/4159m4tp/3561over.html) | Network interface Synchronous Serial | 4xSerial |
| [PA-8T](https://www.cisco.com/c/en/us/products/interfaces-modules/pa-8t-eight-serial-port-adapter-cisco-7000-series-routers/index.html) | Network interface Synchronous Serial | 8xSerial|
| [PA-4E](https://www.cisco.com/c/en/us/td/docs/interfaces_modules/port_adapters/install_upgrade/ethernet/pa-4e_10baset_install_config/pa_4e/3493over.html) | Ethernet network interface | 1xEth (10Mb) |
| [PA-8E](https://www.cisco.com/c/en/us/td/docs/interfaces_modules/port_adapters/install_upgrade/ethernet/pa-8e_10baset_install_config/pa_8e/3494over.html) | Ethernet network interface | 1xEth (10Mb) |
| [PA-POS-OC3](https://www.cisco.com/c/en/us/td/docs/interfaces_modules/port_adapters/install_upgrade/pos/pa-pos-oc3_install_config/paposoc3/3577over.html) | Optical interface OC3 | 1xOC3 |

```
NOTE: Data obtained from Cisco.com. For more information, click on the interface name to go to the Cisco website and get the data for each interface.
```
  
Different interfaces can be selected for each slot. Once selected, click `Next`:

<p align="center">
  <img src="https://i.ibb.co/Q60mVn7/slot.jpg" width="400" />

To finish the router configuration, we look for an Idle-PC which aims to optimise the resources of our equipment (PC, laptop, server, etc.).

<p align="center">
  <img src="https://i.ibb.co/K2SNkyz/slot2.jpg" width="400" />

If a green Idle-PC value is NOT displayed, click the `Idle-PC finder` button to find an Idle-PC value:

<p align="center">
  <img src="https://docs.gns3.com/img/getting-started/setup-wizard-local-server/24.jpg" width="400" />

If you selected the `Idle-PC finder` button (only necessary if no value was automatically detected), GNS3 will calculate a value:

<p align="center">
  <img src="https://i.ibb.co/BHhfVnp/slot6.jpg" width="400" />


(note that this may take a few minutes, depending on the speed of your PC) An Idle-PC value is displayed. Click `OK` to complete:

<p align="center">
  <img src="https://i.ibb.co/k3xtf3L/slotfinal.jpg" width="400" />

```
⚠ IMPORTANT:
If no Idle-PC value is displayed, try clicking the Idle-PC finder button again. You may also need to restart the computer and try again if no value is found. It is incredibly important to have an Idle-PC value when using IOS compatible images. Without this value, DynaMIPS cannot prevent an instance of an IOS image from consuming 100% of a CPU core or hardware thread (in the case of hyperthreading capable CPUs).
```

Click `Finish` to complete the GNS3 Setup Wizard:


<p align="center">
  <img src="https://i.ibb.co/MCNnn0s/finalslot.jpg" width="400" />

In this case, the IDLE PC value has already been specified, according to the value shown on this page, so you can click `Finish`, instead of going through the IDLE-PC search process.

The Preferences window appears, showing the settings you have configured through the Configuration Wizard. Click `Apply` and `OK`.

<p align="center">
  <img src="https://i.ibb.co/MndjHxF/aplicslot.jpg" width="400" />

***`Congratulations`, you are now ready to create your first GNS3 topologies!***

&nbsp;

<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/210186277-0d434bb0-80c0-43a9-b6b0-2e42e18c31a9.png" width="400" />
</p>
</p>
<p align="center">Copyright &copy; 2023-present <a href="https://github.com/gherrada22" target="_blank">George Herrada Farfán</a>
