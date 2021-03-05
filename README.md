# Illustrated guide to build a tiny Homelab
Building a low power hyperconverged Homelab on a tight budget.

## Physical Infrastructure
Detailed description of hardware used in this project.

### Rack and cooling

<p align="center">
  <img width="300" src="https://www.legrand.com/ecatalogue/media/catalog/product/cache/4/image/650x650/9df78eab33525d08d6e5fb8d27136e95/6/4/646230_pw_238615_pz.jpg"><br />
  Legrand 646230
</p>

[Legrand's Linkeo 10" (646230) compact cabinet](https://www.legrand.com/ecatalogue/646230-linkeo-10-compact-cabinet-capacity.html) may provide just enough room to host up to 3-4 USFF PCs, a small UPS unit, and minimal networking equipment. It also provides minimal cooling and cable management capabilities. Cable entry cutouts can be found on the top, bottom, and rear. It also comes with a brush for cable entries.

Removing the uprights may provide more space in exchange of less separation between the installed devices.

<p align="center">
  <img width="300" src="https://www.arctic.de/media/92/9d/52/1613554238/F12_PWM_G00.png"><br />
  Arctic F12 PWM Rev4
</p>  

The top ventillation perforation can accommodate a 120mm fan. You can save some space if you install it on the outside of the box. Using a PWM fan may enable you to control the speed (=noise) levels. This will require one of your USFF PC's to be capable of controlling the fan. A cheap fan like the [Arctic F12 PWM Rev4](https://www.arctic.de/en/F12-PWM/AFACO-120P2-GBA01) may provide enough basic cooling facilities.

Additional cooling can be hacked on the cable entry cutouts. You may want to use smaller fans (e.g., less than 80mm).


### Uninterruptible Power Supply

<p align="center">
  <img width="300" src="https://download.schneider-electric.com/files?p_File_Name=SPD_CLII-9QTM2C_FL_V_520x520.JPG&p_Doc_Ref=SPD_CLII-9QTM2C_FL_V"><br />
  APC Back UPS BX700U-GR
</p>

Installing a UPS into a compact cabinet can be tricky. The [APC Back UPS BX700U-GR](https://www.apc.com/shop/hu/hu/products/APC-Back-UPS-700-VA-230-V-AVR-SCHUKO-aljzatok/P-BX700U-GR) may fit the Legrand cabinet much better without the rack's uprights installed. Laying it on it's side, on the bottom of the cabinet may save some space.

> Ensure that you have proper cooling in your rack before using the UPS unit. Failing to do this can lead to overheating, which may reduce the lifetime of the battery in the UPS.


### Network devices

This setup describes a low budget networking setup. No WLANs or network separation of any sorts.

#### WAN ISP Router

Standard issue WAN ISP fiber router with 1 Gbe uplink and a handful of gigabit ethernet ports. For best results disable all services and Wi-Fi. Turn on automatic updates. Change all passwords. Use it as a basic modem and wired router. Check on it periodically to ensure that the latest firmware is installed and services and WiFi remained turned off.

> TODO: automate this.

#### LAN unmanaged switch

<p align="center">
  <img width="300" src="https://static.tp-link.com/TL-SG1008D(UN)8.0-04_1499931192439k.jpg"><br />
  TP-Link TL-SG1008D switch - back
</p>

Almost any cheap unmanaged gigabit switch will do a fantastic job in this setup. As an example the [TP-Link TL-SG1008D switch](https://www.tp-link.com/us/home-networking/8-port-switch/tl-sg1008d/) has eight gigabit ports, consumes almost no power and it requires no configuration. It is also super cheap.

#### WLAN Access Point

You may want to use a device that can take advantage of the higher bandwidth. Wi-Fi 6 devices are broadly available as of 2021. Setting these up should be fairly straightforward:

- Set the device up in bridge mode (i.e. do not use routing/NAT)
- Turn off all services
- Use the highest available encryption
- Use long passphrases as passwords
- Keep the firmware up-to-date


#### WLAN Rescue Access Point

This can be useful in case if your Proxmox cluster is unavailable.

### Servers


## Host Operating Systems

### Proxmox Virtual Environment

### Armbian


## Clustering

### Corosync

### GlusterFS


## Guest Systems

### Network services
#### NAT
#### DHCP and DNS

### OpenVPN

### TICK stack

### Home Automation
#### Homebridge
#### Hassio

### Ansible AWX
