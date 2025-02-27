# 308: The One About GPU Passthrough

<iframe src="https://player.fireside.fm/v2/RUkczH-V+9ZRzR3sB?theme=dark" width="740" height="200" frameborder="0" scrolling="no"></iframe>

* Air Date: 2019-07-02
* Duration: 56 mins 46 secs

## About this episode

Our crew walks you through their PCI Passthrough setups that let them run Windows, macOS, and distro-hop all from one Linux machine.

## Your hosts
* [Chris Fisher](https://linuxunplugged.com/hosts/chrislas)
* [Wes Payne](https://linuxunplugged.com/hosts/wes)
* [chzbacon](https://linuxunplugged.com/hosts/chzbacon)
* [Alex Kretzschmar](https://linuxunplugged.com/guests/alexktz)

## Sponsored by

None



## Episode links

  * [Windows VirtIO Drivers](https://www.linux-kvm.org/page/WindowsGuestDrivers/Download_Drivers "Windows VirtIO Drivers") — 64-bit versions of Windows Vista and newer require the drivers to be digitally signed.
  * [Alex's arch-vfio-ovmf scripts](https://github.com/IronicBadger/arch-vfio-ovmf "Alex's arch-vfio-ovmf scripts") — Arch Linux installation and VFIO setup scripts 
  * [Looking Glass - Quickstart Guide](https://looking-glass.hostfission.com/quickstart "Looking Glass - Quickstart Guide") — These guides are designed to help you get Looking Glass up and running on an already configured QEMU KVM Virtual Machine that has a VGA PCI Passthrough device. 
  * [duncanthrax/scream](https://github.com/duncanthrax/scream#using-ivshmem-between-windows-guest-and-linux-host "duncanthrax/scream") — Scream is a virtual device driver for Windows that provides a discrete sound device. Audio played through this device is published on your local network as a PCM multicast stream. 
  * [ACS patch COPR](https://copr.fedorainfracloud.org/coprs/jlay/kernel-acspatch/ "ACS patch COPR") — Fedora kernels with add-acs-overrides patch from Arch AUR
  * [ACS Override Kernel Builds](https://queuecumber.gitlab.io/linux-acs-override/ "ACS Override Kernel Builds") — This page contains links to the latest kernel builds with the ACS override patch applied for PCI devices. 
  * [natalie-/fedora-acs-override](https://github.com/natalie-/fedora-acs-override "natalie-/fedora-acs-override") — Using the ACS override patch for Fedora
  * [VFIO tips and tricks: IOMMU Groups, inside and out](https://vfio.blogspot.com/2014/08/iommu-groups-inside-and-out.html "VFIO tips and tricks: IOMMU Groups, inside and out") — Sometimes VFIO users are befuddled that they aren't able to separate devices between host and guest or multiple guests due to IOMMU grouping and revert to using legacy KVM device assignment, or as is the case with may VFIO-VGA users, apply the PCIe ACS override patch to avoid the problem. Let's take a moment to look at what this is really doing. 
  * ["Error 43: Driver failed to load" on Nvidia GPUs passed to Windows VMs](https://wiki.archlinux.org/index.php/PCI_passthrough_via_OVMF#%22Error_43:_Driver_failed_to_load%22_on_Nvidia_GPUs_passed_to_Windows_VMs ""Error 43: Driver failed to load" on Nvidia GPUs passed to Windows VMs") — Since version 337.88, Nvidia drivers on Windows check if an hypervisor is running and fail if it detects one, which results in an Error 43 in the Windows device manager. Starting with QEMU 2.5.0 and libvirt 1.3.3, the vendor_id for the hypervisor can be spoofed, which is enough to fool the Nvidia drivers into loading anyway.
  * [Mac OS Adds Early Support for VirtIO, Qemu - The Passthrough POST](https://passthroughpo.st/mac-os-adds-early-support-for-virtio-qemu/ "Mac OS Adds Early Support for VirtIO, Qemu - The Passthrough POST") — In a new development uncovered by Qemu developer Gerd Hoffmann, Apple has apparently added early support for VirtIO and framebuffer graphics in a later Mac OS Mojave release. 
  * [New and Improved Mac OS Tutorial, Part 1 (The Basics) - The Passthrough POST](https://passthroughpo.st/new-and-improved-mac-os-tutorial-part-1-the-basics/ "New and Improved Mac OS Tutorial, Part 1 \(The Basics\) - The Passthrough POST") — Due to certain recent developments, It’s become clear to us that it’s necessary to update and improve our OSX VM guide. A lot’s changed since we wrote it, and rolling in those changes will make the process much more user friendly and accessible to newer VFIO users. 
  * [Mac OS VM Guide Part 2 (GPU Passthrough and Tweaks) - The Passthrough POST](https://passthroughpo.st/mac-os-vm-guide-part-2-gpu-passthrough-and-tweaks/ "Mac OS VM Guide Part 2 \(GPU Passthrough and Tweaks\) - The Passthrough POST") — We’ve made every attempt to make this as straightforward as possible, but there’s a lot more ground to cover here than in the first part of the guide
  * [UGREEN USB 3.0 Sharing Switch Selector 4 Port 2 Computers Peripheral Switcher Adapter Hub for PC, Printer, Scanner, Mouse, Keyboard with One Button Swapping](https://www.amazon.com/UGREEN-Selector-Computers-Peripheral-Switcher/dp/B01N6GD9JO/ref=sr_1_3?keywords=usb+switcher&qid=1561573709&s=gateway&sr=8-3 "UGREEN USB 3.0 Sharing Switch Selector 4 Port 2 Computers Peripheral Switcher Adapter Hub for PC, Printer, Scanner, Mouse, Keyboard with One Button Swapping") — This USB Switch 4 Port device allows up to 2 users to share 4 USB 3.0 peripheral devices, such as printer,scanner,mouse,keyboard or usb disk etc without the need to constantly swap cables or set up complicated network sharing software. It's a great for use at home if you have multiple PCs or Macs.
  * [How to setup VFIO GPU passthrough using OVMF and KVM on Arch Linux](https://blog.linuxserver.io/2017/04/28/how-to-setup-vfio-gpu-passthrough-using-ovmf-and-kvm-on-arch-linux/ "How to setup VFIO GPU passthrough using OVMF and KVM on Arch Linux") — This article will detail the steps required to passthrough your GPU to a guest VM which will in our case be a Windows 10 VM used for gaming. Yes, this is the exact same technology made popular by Linus on his LinusTechTips YouTube channel in the seven gamers, one CPU video.
  * [Chris' HDMI Monitor 1920x1080 16: 9 LCD Screen](https://www.amazon.com/gp/product/B0762NKY3D/ "Chris' HDMI Monitor 1920x1080 16: 9 LCD Screen")
  * [Lenovo G0A10170UL Thunderbolt 3 Graphics Dock](https://www.amazon.com/Lenovo-G0A10170UL-Thunderbolt-Graphics-Dock/dp/B079JFW3YT "Lenovo G0A10170UL Thunderbolt 3 Graphics Dock") — Amplify your ultrabook’s graphics performance with the integrated NVIDIA GeForce GTX 1050 graphics card. 
  * [Mantiz Venus MZ-02 External Graphic Enclosure eGPU](https://www.amazon.com/gp/product/B0745H6GTX/ref=ppx_yo_dt_b_asin_title_o09_s00?ie=UTF8&psc=1 "Mantiz Venus MZ-02 External Graphic Enclosure eGPU") — Connects Full High Full Length 120" Width 2.5 PCIE Desktop Power GPU to computer WITH an Intel Certified Thunderbolt 3 port.
  * [Synergy](https://symless.com/synergy "Synergy") — Synergy is a software download that shares one mouse and one keyboard between multiple computers. Simply move your mouse between your computers effortlessly
  * [barrier: Open-source KVM software](https://github.com/debauchee/barrier "barrier: Open-source KVM software") — Barrier is KVM software forked from Symless's synergy 1.9 codebase. Synergy was a commercialized reimplementation of the original CosmoSynergy written by Chris Schoeneman. 
  * [foxlet/macOS-Simple-KVM](https://github.com/foxlet/macOS-Simple-KVM/ "foxlet/macOS-Simple-KVM") — Documentation to set up a simple macOS VM in QEMU, accelerated by KVM. 



## Tags

[acs](https://linuxunplugged.com/tags/acs), [code 43](https://linuxunplugged.com/tags/code%2043), [egpu passthrough](https://linuxunplugged.com/tags/egpu%20passthrough), [iommu group](https://linuxunplugged.com/tags/iommu%20group), [jupiter broadcasting](https://linuxunplugged.com/tags/jupiter%20broadcasting), [linux podcast](https://linuxunplugged.com/tags/linux%20podcast), [linux unplugged](https://linuxunplugged.com/tags/linux%20unplugged), [looking glass](https://linuxunplugged.com/tags/looking%20glass), [macos simple kvm](https://linuxunplugged.com/tags/macos%20simple%20kvm), [macos virtio](https://linuxunplugged.com/tags/macos%20virtio), [mantiz venus](https://linuxunplugged.com/tags/mantiz%20venus), [ovmf](https://linuxunplugged.com/tags/ovmf), [pfsense with pci passthrough](https://linuxunplugged.com/tags/pfsense%20with%20pci%20passthrough), [uefi firmware](https://linuxunplugged.com/tags/uefi%20firmware), [vfio](https://linuxunplugged.com/tags/vfio), [virt-manager](https://linuxunplugged.com/tags/virt-manager)