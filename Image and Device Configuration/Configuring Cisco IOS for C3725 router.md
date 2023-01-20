<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/211248683-9e2e62cf-cd80-4137-9861-f97980405faa.png" alt="Icono de GNS3">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/210186277-0d434bb0-80c0-43a9-b6b0-2e42e18c31a9.png" width="400" />
</p>

## 🔱 Configuring Cisco IOS for C3725 router.

- If you are a network engineer you must know the most famous network simulator GNS3. From here you can download the Cisco C3725 series IOS for GNS3. But before I give you the download link, I want to discuss some features and advantages of GNS3 over the other network simulators.

- GNS3 is a graphical network simulator where you can create and build simple and complex network scenarios on your computer virtually. In this way, you test your configuration before implementing it in the real network. You can use different network devices with GNS3 such as routers, virtual PC, cloud, etc. [Here for more information](https://github.com/gherrada22/GNS3-Guide)

- A Cisco C3725 switch/router is a network device that provides switching and routing functions. Switching allows multiple devices to connect to a network and communicate with each other, while routing allows data packets to be routed from one network to another. The C3725 is a Cisco-specific model that is capable of supporting several routing protocols, including OSPF, EIGRP, BGP and RIP.

- It also supports various switching protocols, such as VLANs and VTP. This device is used in enterprises and organisations to connect and manage local and wide area networks. [Here is the link for GNS3 Switch IOS](https://github.com/gherrada22/GNS3-Guide/tree/main/Image%20and%20Device%20Configuration/Download%20%20IOS%20Cisco).


## ✅ Import Image in GNS3

In the GNS3 GUI, click `Edit > Preferences` to open the Preferences menu.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-48.png" width="400" />

In `Dynamips`, click on `IOS routers`. All the routers/switches we have added to GNS3 will appear on the right. Click on `New` to add a new router.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-49.png" width="400" />

Select `New Image` and click `Browse...`

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-50.png" width="400" />

Select the .bin file of the Cisco router image to install, in our case c3725-adventerprisek9-mz.124-25d.bin:

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-64.png" width="400" />

If it is compatible, GNS3 will indicate with a message if we want to decompress the IOS image, click `Yes`.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-52.png" width="400" />

The wizard will decompress the .bin into a .image (c3725-adventerprisek9-mz.124-25d.image), click `Next`.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-65.png" width="400" />


The new IOS router installation wizard will show us the name and platform of the c3725. At this point in the installation we can choose between leaving the device as a router (the default option) or converting it into a switch (it will not have the advanced options of a router, but it will have the necessary and basic options for VLAN, spanning tree, etc.). In our case, since we want it to be a switch only, we will check `This is an EtherSwitch router`. Enter the name (in name), for example `c3725_Switch` and click `Next`.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-69.png" width="400" />


We will choose the RAM to be assigned to the virtual router, by default 128MiB.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-67.png" width="400" />


Finally, we will choose the type of adapter for each slot. In the case of this IOS for the C3725, slot 0 must have the GT96100-FE type and slot 1 the NM-16ESW type (16-port EtherSwitch network module). In slot 2 we can choose between NM-1FE-TX (1-port Fast Ethernet network module (100BASE-TX interface)) or NM-4T (4-port serial network module). In our case we will leave it.

- Slot 0: GT96100-FE
- Slot 1: NM-16ESW
- Slot 2: NM-1FE-TX

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-68.png" width="400" />

We can also add WIC modules, which are serial port adapters. It is not necessary, but we will add some in case we need them in the future.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-70.png" width="400" />

Choose the Idle-PC for this IOS (it can be 0x602467a4) and click `Finish`.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-71.png" width="400" />

If everything is correct, it will add it as a switch (which is what we have chosen). Click on `OK`.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-72.png" width="400" />

If you have chosen switch, it will be available in Switches.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-73.png" width="400" />

And note that ports Fa0/0 and Fa0/1 will only be routable interfaces.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-74.png" width="400" />

And port Fa1/0 to Fa1/15 will be "normal" switch interfaces.

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-75.png" width="400" />

If we have added WIC ports they will appear as "Serial...".

<p align="center">
  <img src="https://proyectoa.com/wp-content/uploads/2022/05/imagen-76.png" width="400" />

***`Congratulations`, you are now ready to create your first GNS3 topologies!***

&nbsp;

<p align="center">
  <img src="https://user-images.githubusercontent.com/104341274/210186277-0d434bb0-80c0-43a9-b6b0-2e42e18c31a9.png" width="400" />
</p>
</p>
<p align="center">Copyright &copy; 2023-present <a href="https://github.com/gherrada22" target="_blank">George Herrada Farfán</a>


