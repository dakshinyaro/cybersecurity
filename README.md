Linux Basic Commands (used after installation)
ls → List files and directories
cd → Change directory
pwd → Show current directory
mkdir → Create a new folder
rm → Remove files
sudo → Run command as administrator
apt update → Update package list
apt upgrade → Upgrade installed packages
lsblk → View disk partitions
fdisk -l → Show partition details
mount → Mount a partition
umount → Unmount a partition
diskpart → Manage disk partitions
list disk → Show disks
list volume → Show partitions
exit → Exit diskpart

Steps to Setup Dual Boot (Windows + Linux)

Step 1: Backup Data
Always take backup of important files before starting.

Step 2: Create Free Space
Open Disk Management in Windows
Shrink an existing drive (C: or D:)
Create at least 20–50 GB free space

Step 3: Create Bootable USB
Download Linux ISO (e.g., Kali Linux / Ubuntu)
Use tools like:
Rufus
Create bootable USB drive

Step 4: Boot from USB
Restart system
Press boot key (F2 / F12 / ESC / DEL)
Select USB device

Step 5: Install Linux
Choose “Install OS”
Select:
“Install alongside Windows” (easy method)
OR
“Manual partitioning” (advanced)

Step 6: Partition Setup (Manual)
Create:
Root (/) → 20GB+
Swap → 2–4GB
Home (/home) → remaining space

Step 7: Install Bootloader (GRUB)
GRUB will automatically detect Windows
It provides OS selection during startup

Step 8: Restart System
After installation, reboot
You will see:
Linux
Windows Boot Manager

What is Learned
Understanding of dual boot concept
Disk partitioning and memory allocation
Bootloader (GRUB) working
Basic Linux commands
OS installation process
System-level configuration

Issues Faced
Boot menu not showing (GRUB issue)
Windows overriding bootloader after update
Partition errors during installation
USB not detected in BIOS
Insufficient disk space
Secure Boot causing installation failure

Solutions to Issues
Reinstall GRUB using live USB
Disable Secure Boot in BIOS
Use correct partition format (ext4)
Ensure proper boot mode (UEFI/Legacy)
Update BIOS settings correctly

Conclusion
Dual booting is a powerful method to use multiple operating systems on a single machine. It helps users explore Linux while keeping Windows for regular use. Though some technical challenges may arise, proper understanding of partitions and bootloaders makes the process smooth and effective.
