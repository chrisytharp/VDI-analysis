# VDI-analysis

VDI Analysis
When you create a virtual machine in VirtualBox you need to create a virtual disk image (VDI) file. This file behaves like a physical hard disk drive (HDD) in that it stores the operating system file systems, and any changes made inside the virtual machine will be stored in this disk image. 

To understand what is on this VDI we can use standard digital forensics tools and techniques, such as Autopsy. Before we can analyse the VDI we must convert it to a format that Autopsy can read. To do this we will use the qemu-img tool.

qemu-img convert -f vdi -O raw inputfile.vdi outputfile.img
