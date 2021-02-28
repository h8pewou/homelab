# Guide to build your tiny Homelab
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

#### LAN unmanaged switch

#### WLAN Access Point

#### WLAN Rescue Access Point


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
