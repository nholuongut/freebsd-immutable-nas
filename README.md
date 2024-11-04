# FreeBSD immutable NAS

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

## Introduction

This repository contains a packer script followed by an Ansible provisioning script for the automated creation of an immutable FreeBSD ISO image for my personal NAS. 

The image is "immutable" in the sense that the root partition is read-only, with particular mount points mounted as in-memory filesystems, allowing for non-persistent writes. Therefore the data saved on the bootable Memory card never changes, and upgrades are done by swapping the card.

Persistent, user data is saved on a ZFS pool.

Build with:

    packer build -var-file=freebsd110.json freebsd.json


This repository has been made public for educational purposes, to provide an example of a working "immutable server", and inspire people to start working on similar architectures. It can also serve as a good read on the basic configuration of FreeBSD as a NAS.


## Hardware (Q4 2014)

 * Lian Li PC-Q25B Mini-ITX
 * Silverstone 300W SST-ST30SF 
 * SuperMicro A2SDi-2C-HLN4F - Mini-ITX Mainboard
 * 1 * 8GB Unbuffered ECC RAM Kingston ValueRAM DDR4-2400 regECC
 * 3 * 4TB WD RED (ZFS pool)
 * 120GB internal SSD Intel SSDSC2BB120G401 DC S3500 Series (ZFS ZIL)
 * SATA - eSATA adapter
 * Inateck USB 3.0 Docking Station + Additional drives for backups through eSATA
 * Be Quiet! Silent Wings PWM 120+140mm

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: Nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)
* [PayPal.me](https://www.paypal.com/paypalme/nholuongut)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟
