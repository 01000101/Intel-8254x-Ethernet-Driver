# Intel 8254x Ethernet Driver Example
Intel 8254x Ethernet Controller Example Driver For Hobby Operating System Developers

## Overview
Writing a custom or hobby driver for the Intel 8254x series Ethernet controllers?  I’ve been down that road before and luckily there are quite a few resources to help you along your journey.  For starters, if you’re not already a member of [OSDev.org](http://osdev.org/) I’d highly recommend joining.  They’re a great community and the wiki and forums contain invaluable resources for the hobby/embedded Operating System developer.


Secondly, you’ll want to grab a copy of the [Intel PCI/PCI-X Family of Gigabit Ethernet Controllers Software Developer’s Manual](http://www.intel.com/content/www/us/en/ethernet-controllers/pci-pci-x-family-gbe-controllers-software-dev-manual.html) which covers the following Ethernet controller chipsets: 82540EP/EM, 82541xx, 82544GC/EI, 82545GM/EM, 82546GB/EB, and 82547xx.  These controllers can be found in products such as the Intel PRO/1000, VMWare ESXi/VS2/Player/Workstation (E1000), QEMU/KVM, and VirtualBox.  This makes the Intel 8254x-series chipset appealing to developers as it’s widely emulated and can be found in a lot inexpensive consumer PCs.  Here’s a link to the Gigabit Ethernet Controllers Software Developer’s Manual.


### Disclaimer
This code isn’t guaranteed to work after a fresh copy and paste.  You may need to do some modifying as, let’s face it, it’s being put into a hobby/embedded/custom OS with I’m sure some very unique design choices which may or may not be within the same mental realm I was in when I wrote this.  Also, this is one of those cases where you should be cautious of emulators and virtualization systems properly mimicking the physical controller’s behavior.  For instnace, if you search around VirtualBox’s code repository you will find my code name 01000101 in there with some patches for the E1000 driver (some minor inconsistencies between real hardware and VirtualBox’s implementation).  Be aware, but don’t underestimate those systems either.  99/100 issues will likely be your own code.
