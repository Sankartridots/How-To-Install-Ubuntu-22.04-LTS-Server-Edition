# How-To-Install-Ubuntu-22.04-LTS-Server-Edition
How To Install Ubuntu 22.04 LTS Server Edition Ubuntu 22.04 LTS Server Installation Guide With Screenshots

Install Ubuntu 22.04 Server Step By Step
Ubuntu is a beginner-friendly Linux distribution, so installing Ubuntu server isn't that difficult. Just follow the steps given below carefully, change some settings according to your requirements and you will be fine.

Step 1 - Boot Ubuntu ISO
Boot your system with the newly created Ubuntu 22.04 bootable USB drive. First, you will see the Grub menu. By default, the first option (i.e. Try or Install Ubuntu Ubuntu Server) is automatically selected to boot into the live system.

Try Ubuntu
Try Ubuntu
Step 2 - Choose Language for Ubuntu Installer
After a few seconds, you will see the language selection window for the installer menu. I choose "English". Hit ENTER to continue.

Choose Installer Language
Choose Installer Language
Step 3 - Keyboard Configuration
Choose your preferred keyboard layout. I go with English US.

Select Keyboard Layout
Select Keyboard Layout
Heads Up: At the bottom of the each installer window, you will see two menus namely "Done" and "Back", which will allow you to go forward to next screen or go back if you want to change any installation options.

Step 4 - Choose Type of Install
Next, choose the base for your installation. You will be given two choices as listed below.

Ubuntu Server - This is the default choice for the base installation. It contains the basic set of packages that is required for a server operating system.
Ubuntu Server (minimized) - This version has been customized to have a minimal runtime OS. This should be usually selected when the humans are not expected to log in.
I go with default choice i.e. Ubuntu Server.

Choose Base for the Installation
Choose Base for the Installation
Step 5 - Configure Network Connections
Next, you to configure at least one network interface, so that your server can be able to communicate with other systems. If you have a working DHCP server on your network, you can simply leave it to get an IP address automatically from the DHCP server. By default, the DHCP option is selected.

Configure Network Interface
Configure Network Interface
If you prefer to manually set an IP address, choose the network interface (E.g. enp6s18) by using the TAB key and hit ENTER to choose "Edit IPv4" from the list.

Choose "Edit IPv4" Option
Choose "Edit IPv4" Option
After choosing "Edit IPv4" option, press ENTER again and then select "Manual" from the IPv4 method list.

Manually Configure IPv4
Manually Configure IPv4
Enter the Subnet, IP address, Gateway and Name servers in the respective column and choose "Save" and hit ENTER to save the network configuration.

Set IP Address for Ubuntu Server
Set IP Address for Ubuntu Server
You will now be redirected to the main network configuration window again. Press the TAB key to choose "Done" and again press ENTER to continue to the next section.

Ubuntu Server Static Network Configuration
Ubuntu Server Static Network Configuration
Step 6 - Configure Proxy
If you Ubuntu server is required a proxy server to access Internet, enter the proxy server details in this window. If proxy server is not required, simply leave it empty and hit ENTER to continue.

Configure Proxy Server Details
Configure Proxy Server Details
Step 7 - Configure Ubuntu Archive Mirror
Here, you can configure an archive mirror for your Ubuntu server. By default, the installer will pick you a suitable, nearest archive mirror for you. If you don't want to use it, you can manually provide an archive mirror.

Configure Ubuntu Archive Mirror
Configure Ubuntu Archive Mirror
Step 8 - Update Installer (Optional)
Next, you will be notified if a new Ubuntu installer is available to download and use for the rest of the installation. It is completely your choice.

If you want to try the new Ubuntu installer, choose "Update to the new installer" option and hit ENTER. The new installer will be downloaded and after that the installation will continue as usual.

If you want to stick with the current Ubuntu installer, select "Continue without updating".

I want to try the new Ubuntu installer TUI, so I chose "Update to the new installer" option.

Ubuntu Installer Update
Ubuntu Installer Update
Heads Up: Please note that the question for selecting Ubuntu installer update option will not be asked in the older Ubuntu 22.04 ISO images.

Step 9 - Disk Partitioning
The next section is important. In this section, you have to choose how you'd like to configure your hard drive. You can let the installer to automatically partition the drive for you or you can manually partition the disk as per your liking.

Step 9.1. - Automatic Partitioning
If you want to automatically partition the disk, simply choose "Use an entire disk" option.

Automatic Partitioning
Automatic Partitioning
You can also choose "Encrypt the LVM group with LUSK" if you want to encrypt your disk. If you chose this option, you will have to provide a passphrase. This will enhance the security and prohibit unauthorized access to your OS.

The installer will choose the best partitioning scheme for you. You don't have do anything.

Disk Partition Summary
Disk Partition Summary
If you are beginner, you can use the automatic partitioning method and this is the default partitioning method.

Heads Up: Note that Ubuntu no longer requires a separate partition for swap space, nor will the automated install create one.


After disk partitions are formatted, skip to the Step 10.

If you prefer manual partition over auto partition, read the next section.

Step 9.2. - Manual Partitioning
This method is for intermediate and advanced users. If you're not happy with auto partitioning method, you can choose "Custom storage layout" to manually partition your disk.

Manual Partitioning
Manual Partitioning
For the purpose of this guide, I will be creating the following partition scheme:

Total disk space - 50 GB.
/boot (EXT4) - 2 GB.
/home (EXT4) - 20 GB.
/ (EXT4) - Remaining space.
Choose free space from the available disk and hit ENTER.

Choose Free Space
Choose Free Space
Choose "Add GPT Partition" from the list and hit ENTER key.

Add GPT Partition
Add GPT Partition
Enter the partition size (E.g. 2G), filesystem type (E.g. EXT4), and the mount point (E.g. /boot) and select "Create" and press ENTER. Please note that you must mention G for GB, and M for MB when defining the partition size.

Create Boot Partition
Create Boot Partition
Now the newly created partition will be shown under the FILE SYSTEM SUMMARY menu. Again, choose the free space and hit ENTER, choose "Add GPT Partition".

Enter the partition size (E.g. 20GB), filesystem type (E.g. EXT4), and the mount point (E.g. /home) and select "Create" and press ENTER.

Create Home Partition
Create Home Partition
Similarly, create the root (/) partition. Select free space -> Add GPT partition. Enter the partition size, filesystem type (E.g. EXT4), and the mount point (E.g. /) and select "Create" and press ENTER. I have assigned the remaining space to the root partition.

Create Root Partition
Create Root Partition
After creating all required partitions, review the disk partition layout. If you are satisfied with current partitioning layout, choose "Done" and hit ENTER to save the changes.

Save Partition Changes
Save Partition Changes
All the data in the disk will be deleted now. Please ensure there is no data in the drive and choose "Continue" to format the disk partitions.

Confirm Formatting Partitions
Confirm Formatting Partitions
Step 10 - Enter Ubuntu Hostname and Username Information
In this section, enter the suitable hostname for your Ubuntu server. And also enter username and password that you will use to log in to your Ubuntu server.

Enter Ubuntu Hostname and Username Information
Enter Ubuntu Hostname and Username Information
Step 11 - Enable Ubuntu Pro
If you have Ubuntu pro account, you can choose "Enable Ubuntu Pro" option. It will upgrade your Ubuntu server to get security updates until 2032.

Enable Ubuntu Pro
Enable Ubuntu Pro
I don't have Ubuntu Pro account, so I skipped this it. You can register with Ubuntu Pro at any time later by entering the following command:

$ sudo pro attach
Step 12 - Configure SSH
In step, you can setup SSH. Check the "Install OpenSSH Server" check-box and choose "Done" and hit ENTER.

Configure SSH
Configure SSH
Step 13 - Select Featured Server Snaps
In the next section, you will be presented with some popular snaps that you may want to install. Choose the snap applications of your choice and hit ENTER to continue. You can select or deselect the apps with the SPACEBAR key.

Featured Server Snaps
Featured Server Snaps
Now the Ubuntu server installation will start. This will download and install a lots of packages. So please be patient.

Installing Ubuntu 22.04 LTS Server
Installing Ubuntu 22.04 LTS Server
Step 14 - Reboot Ubuntu Server
Once the Ubuntu server installation is completed, select "Reboot Now" option and hit ENTER to reboot your Ubuntu server.

Reboot Ubuntu Server
Reboot Ubuntu Server
Congratulations! Ubuntu 22.04 LTS server is successfully installed!

Log in to Ubuntu Server
Log in to your newly installed Ubuntu server. Enter the username and its password which you created during the installation process.

Login to Ubuntu Server
Login to Ubuntu Server
Start using your newly installed Ubuntu 22.04 LTS server edition.

Update Ubuntu
The first thing after installing any OS is to update it. Ubuntu is no exception. Let us update the Ubuntu server by entering the following commands:

$ sudo apt update
$ sudo apt full-upgrade
Update Ubuntu Server
Update Ubuntu Server
During the installing updates task, you will be prompted to restart some services. Choose OK to do so.

Restart Services
Restart Services
After all updates are applied, remove any leftover, unnecessary packages by running the following commands:

$ sudo apt autoremove
$ sudo apt autoclean
Finally, once again reboot your system.

$ sudo reboot
Conclusion
In this step by step tutorial, we learned how to download latest Ubuntu 22.04 LTS server version and how to create a Ubuntu bootable USB drive using the ISO and finally how to install Ubuntu 22.04 LTS server edition with screenshots.
