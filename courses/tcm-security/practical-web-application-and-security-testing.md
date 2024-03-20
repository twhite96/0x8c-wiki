---
description: >-
  There is some base knowledge you should have before attempting to go through
  this course:
---

# 🛡️ Practical  Web Application and Security Testing

* Command Line knowledge
* How networks work (very basic knowledge)
* Some familiarity with Linux and Python
* Feel comfortable with how servers and web apps work
* Have a machine with enough memory, disk storage, and CPU to run multiple VMs at once.



### Setup for Apple M-SeriesChip users



The course is Windows-centric in that it gives tools that work well for Windows. There are still tools shown in the course for Linux and macOS like VirtualBox, but Virtualbox does not have a VM solution for Apple ARM devices running the M-Series chips.



In this entry I will show you were to get the tools you need to virtualize your lab on an M1 Mac.



### VM Solutions



VMWare has a solution called [VMWare Fusion](https://customerconnect.vmware.com/downloads/info/slug/desktop\_end\_user\_computing/vmware\_fusion/13\_0) that has an M1 client you need to license but can use for free. It is a good, robust solution for many things, and if you have a powerful M2-M3 Max and/or Ultra chip in your Mac, I would suggest using this; it just has more features.

For us M1 plebs, however, there is a simpler solution that is lightweight enough to run on the M1 called [UTM](https://github.com/utmapp/UTM), which uses Apple's new-ish virtualization framework.



### The OSes You'll Need

{% hint style="info" %}
[UTM has its own gallery that you can browse to install most of the VMs used in this course. However, an ISO is probably your best bet.](#user-content-fn-1)[^1]
{% endhint %}

There are two VMs you'll need ISOs for:

* Kali Linux
* Ubuntu Server

On the Ubuntu Server, you will install Docker, which is another piece of software we'll need for this course.



You can download the ISO of Kali Linux [on their website](https://www.kali.org/get-kali/#kali-installer-images) or directly from the links below:

* [Kali ISO](https://cdimage.kali.org/kali-2024.1/kali-linux-2024.1-installer-arm64.iso)
* [Kali Torrent File](https://cdimage.kali.org/kali-2024.1/kali-linux-2024.1-installer-arm64.iso.torrent)

You can download Ubuntu Server [on their website](https://ubuntu.com/download/server/arm) which will take you to the page for the correct architecture. If you download the wrong ISO file, say AMD64 instead of ARM64, these ISO files will not boot.



### Installing Kali Linux



This tripped me up a bit. I watched a YouTube video on it but found that Kali has documentation on how to install Kali inside of UTM, which you can find on their [documentation page](https://www.kali.org/docs/virtualization/install-utm-guest-vm/). If you're still stumped, I've linked the video below.



{% embed url="https://youtu.be/U09soewiu18" %}



[^1]: 
