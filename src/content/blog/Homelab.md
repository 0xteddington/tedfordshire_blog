---
title: '$ ~/homelab.conf'
description: 'My Homelab V1'
pubDate: 'Feb 21 2022'
heroImage: '/blog-placeholder-2.jpg'
---

There are many ways of learning skills in technology and personally, I like to learn by practical vs theory, and installing an application or installing hardware can be one of the best ways to get hands-on experience.

However, we don’t all have access to enterprise equipment and a large data centre with full network stacks and aircon to keep it all cool.

But you can get pretty close these days with VMs, Cloud infra and some old hardware from eBay or old computer fairs.

Here is a rundown of my home lab setup to help those looking for some inspiration.

---

### Servers

**Micro Form Factors**

These small PCs, running laptop components are great as you get some good power from the CPU and RAM without running a huge power bill and can be headless (no screen attached). The downside to these is the lack of expansion so you have to be clever if you want to add things like a second network card. USB ethernet adapters are a great way to add secondary network connections.

From £100 – £500 for an 8-core processor device for running VMs

---

The HP was my only Windows device until I got my new PC, and was used for all those things sometimes you just have to use Windows.

> ==Make: HP  
> Model: Elite desk 800 G5  
> OS: Windows 10 Pro  
> CPU: Intel i5-9500T 6 Core 3.70 GHz  
> GPU: Intel UHD 630  
> SSD: 500 GB Nvme M.2 Western Digital Blue  
> MEM: 16 GB DDR4==

The Lenovo is running the Debian server as my Plex media server attached to the Synology NAS which holds the media.

> ==Make: Lenovo  
> Model: Think station m910q  
> OS: Ubuntu 20.04  
> CPU: Intel i5-6500T 6 Core 3.1 GHz  
> GPU: Intel UHD 530  
> SSD: 500 GB 2.5 Crucial MX500  
> MEM: 8 GB DDR4==

The Dell runs as my daily driver Linux device with my local Kali VM for Hack the Box and Try Hack Me training.

> ==Make: Dell  
> Model: OptiPlex 3080  
> OS: Ubuntu Budgie 20.04  
> CPU: Intel i5-10500T 6 Core 3.80 GHz (12 Threads)  
> GPU: Intel UHD 630  
> SSD: 500 GB Nvme M.2 Western Digital Blue  
> SSD: 500 GB 2.5 Crucial MX500  
> MEM: 16 GB DDR4==

The Raspberry Pi 4b is running [Monero](https://www.getmonero.org/) (XMR) Crypto mining.

>   
> ==Make: Raspberry Pi  
> Model: Pi 4 Model B  
> OS: Raspberry Pi OS 64 Bit  
> MEM: 8 GB  
> SD: 32 GB SanDisk==

**Workstation**

Designed for graphics or intense computing, these workstations are generally built using server components but generally with a lack of ECC Memory and redundant power supplies.

> ==Make: HP  
> Model: z320  
> OS: Ubuntu Server 20.04  
> CPU: Intel Xeon 1245 v3 4 Core 3.8 GHz (8 Threads)  
> GPU: NVIDIA GeForce 750 TI  
> SSD: 500 GB 2.5 Crucial MX500  
> HDD: 1TB 3.5 7200 rpm Seagate BarraCuda  
> MEM: 16 GB DDR3==

The HP Z230 is running Observium, Syslog, Splunk and other applications for monitoring my devices and networks, as well as Hashcat Password cracker to make use of the GPU.

---

### Network Attached Storage (NAS)

[NAS](https://en.wikipedia.org/wiki/Network-attached_storage) are small computers/units that can hold a number of disks together and provide redundancy such as [RAID](https://en.wikipedia.org/wiki/RAID) and application services. As the name suggests these devices sit on your network are the PCs or Servers connected to them using protocols such as SMB, NFS or CIFS.

My Synology NAS holds my media collection for my Plex Media Server, while my QNAP holds everything else from logs to documents, pictures and code.

> ==Make: QNAP  
> Model: TS-653A  
> OS: QTS 5.0.0  
> CPU: Intel Celeron N3150 4 Core 1.60 GHz  
> MEM: 8 GB DDR2  
> HDD: 6x Toshiba 1 TB 5400 NAS Drives==

> ==Make: Synology  
> Model: DS218 Play  
> OS: Synology DSM 7.0.1  
> CPU: Realtek 1.4 4 Cores  
> MEM: 1 GB DDR4  
> HDD: 2x Toshiba 6 TB 5400 NAS Drives==

---

### Network

This is where generally it can get expensive and spending a little more money here will be better in the long run. That’s not to say that there aren’t some bargains out there to be had.

> ==Netgear 8 Port 1Gbps switch  
> Devolo dLAN® 1200+ Powerline Adapters  
> UniFi Dream Machine Router==

The router and Wifi run in the living room with the ISP-provided kit in modem-only mode. Then the powerlines provide a connection into the office and the 8 port switch to connect the lab together.

---

### General PC

My everyday PC, where I can play games and run VMs locally for various training and learning. I can highly recommend [SCAN](https://www.scan.co.uk/) as a supplier they have always had great customer service, delivery and reasonable prices. I have used them for over 15 years now and they have never faulted me.

> ==Make: 3XS Gamer Ti  
> OS: Windows 11 Home  
> CPU: Intel Core i7 12700K CPU.  
> Memory/RAM: 32GB Corsair Vengeance RGB PRO 3600MHz DDR4.  
> GPU: 8GB ASUS GeForce RTX 3060 Ti TUF GAMING OC V2 GDDR6.  
> Motherboard: ASUS PRIME Z690-P WIFI D4.  
> SSD: 2x 1TB Samsung 980 M.2 NVMe SSD.==

**Monitors**

> ==2x LG 35″ 35WN75C-B 3440×1440 VA 100Hz FreeSync sRGB99 HDR10 Curved LED Backlit Ultrawide Gaming Monitor==

**Accessories**

> ==Steel Series Apex 3 TKL Keyboard==
> 
> ==Steel Series Aerox 3 Wireless Mouse==
> 
> ==Creative Labs Pebble V3 Speakers==

---

## The Future

I have some enterprise-grade devices that I have collected over the last couple of years to expand my VM capabilities and allow me to spin up more VMs to work with when learning.

I can then expand the network and run fibre from the garage to the office and segregate the lab network from the home network eventually.

> ==CISCO 3650 Catalyst Switch 24 Port  
> CISCO 3850 Catalyst Switch 48 Port  
> Dell PowerEdge R710==

Hope this gives you some idea of running a home lab, with a small and relatively cheap kit.

Ted.

