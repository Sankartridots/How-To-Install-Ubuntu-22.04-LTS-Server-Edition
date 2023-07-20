# How-To-Install-Ubuntu-22.04-LTS-Server-Edition
How To Install Ubuntu 22.04 LTS Server Edition Ubuntu 22.04 LTS Server Installation Guide With Screenshots

Install Ubuntu 22.04 Server Step By Step
Ubuntu is a beginner-friendly Linux distribution, so installing Ubuntu server isn't that difficult. Just follow the steps given below carefully, change some settings according to your requirements and you will be fine.

Step 1 - Boot Ubuntu ISO
Boot your system with the newly created Ubuntu 22.04 bootable USB drive. First, you will see the Grub menu. By default, the first option (i.e. Try or Install Ubuntu Ubuntu Server) is automatically selected to boot into the live system.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/d315bef7-2466-4b64-a1f4-9ba963b66842)


Step 2 - Choose Language for Ubuntu Installer

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/bf0a9dc7-1620-4b05-a2a2-84a357de8b9f)


Step 3 - Keyboard Configuration

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/b9ba26d7-3df4-46c9-9048-01e631c72fb8)


Step 4 - Choose Type of Install

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/af9f6102-4372-4006-8e44-a11c7a8dba82)


Step 5 - Configure Network Connections

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/401b9bfa-f076-4df8-b565-98f673659887)


Next, you to configure at least one network interface, so that your server can be able to communicate with other systems. If you have a working DHCP server on your network, you can simply leave it to get an IP address automatically from the DHCP server. By default, the DHCP option is selected.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/258b4888-ac22-4aa9-877f-7c3b770342c8)


If you prefer to manually set an IP address, choose the network interface (E.g. enp6s18) by using the TAB key and hit ENTER to choose "Edit IPv4" from the list.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/79aa02a1-ce83-4630-a655-a4df14b5f2ba)


After choosing "Edit IPv4" option, press ENTER again and then select "Manual" from the IPv4 method list.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/4a1c4290-da8d-460e-8ea5-71a3b7e8b728)


Enter the Subnet, IP address, Gateway and Name servers in the respective column and choose "Save" and hit ENTER to save the network configuration.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/9056ecca-50da-4a96-84bc-d1bd0de2819f)


You will now be redirected to the main network configuration window again. Press the TAB key to choose "Done" and again press ENTER to continue to the next section.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/a08bd20b-7c6a-4142-b3fa-85ec30f068e3)


Step 6 - Configure Proxy
If you Ubuntu server is required a proxy server to access Internet, enter the proxy server details in this window. If proxy server is not required, simply leave it empty and hit ENTER to continue.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/b25b9bdb-155e-4838-b1b3-95a88aed5dcb)


Step 7 - Configure Ubuntu Archive Mirror
Here, you can configure an archive mirror for your Ubuntu server. By default, the installer will pick you a suitable, nearest archive mirror for you. If you don't want to use it, you can manually provide an archive mirror.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/d6de7d7c-e59a-4717-ad2d-9ff385362282)


Step 8 - Update Installer (Optional)
Next, you will be notified if a new Ubuntu installer is available to download and use for the rest of the installation. It is completely your choice.

If you want to try the new Ubuntu installer, choose "Update to the new installer" option and hit ENTER. The new installer will be downloaded and after that the installation will continue as usual.
If you want to stick with the current Ubuntu installer, select "Continue without updating".
I want to try the new Ubuntu installer TUI, so I chose "Update to the new installer" option.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/c2b15f01-ea91-46f7-a205-358e91181945)


Heads Up: Please note that the question for selecting Ubuntu installer update option will not be asked in the older Ubuntu 22.04 ISO images.

Step 9 - Disk Partitioning
The next section is important. In this section, you have to choose how you'd like to configure your hard drive. You can let the installer to automatically partition the drive for you or you can manually partition the disk as per your liking.

Step 9.1. - Automatic Partitioning
If you want to automatically partition the disk, simply choose "Use an entire disk" option.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0a712d8e-be51-4474-9482-5d73ebc4f3c4)

You can also choose "Encrypt the LVM group with LUSK" if you want to encrypt your disk. If you chose this option, you will have to provide a passphrase. This will enhance the security and prohibit unauthorized access to your OS.

The installer will choose the best partitioning scheme for you. You don't have do anything.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/e42ca4a6-fa99-4c09-b012-3392797ca4e0)


If you are beginner, you can use the automatic partitioning method and this is the default partitioning method.

Heads Up: Note that Ubuntu no longer requires a separate partition for swap space, nor will the automated install create one.


After disk partitions are formatted, skip to the Step 10.

If you prefer manual partition over auto partition, read the next section.

Step 9.2. - Manual Partitioning
This method is for intermediate and advanced users. If you're not happy with auto partitioning method, you can choose "Custom storage layout" to manually partition your disk.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/999fd3b8-d8cb-4c3b-a301-54c41ae0213d)


For the purpose of this guide, I will be creating the following partition scheme:

Total disk space - 50 GB.
/boot (EXT4) - 2 GB.
/home (EXT4) - 20 GB.
/ (EXT4) - Remaining space.
Choose free space from the available disk and hit ENTER.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/986f2dce-4a1e-4943-8446-463a91b1d250)


Choose "Add GPT Partition" from the list and hit ENTER key.

https://ostechnix.com/wp-content/uploads/2023/04/Add-GPT-Partition.png

Enter the partition size (E.g. 2G), filesystem type (E.g. EXT4), and the mount point (E.g. /boot) and select "Create" and press ENTER. Please note that you must mention G for GB, and M for MB when defining the partition size.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/10696006-6b50-4eab-aa8c-707f678e972e)


Now the newly created partition will be shown under the FILE SYSTEM SUMMARY menu. Again, choose the free space and hit ENTER, choose "Add GPT Partition".

Enter the partition size (E.g. 20GB), filesystem type (E.g. EXT4), and the mount point (E.g. /home) and select "Create" and press ENTER.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/28d0382c-32a7-4891-a9d7-930a2b7abc8b)


Similarly, create the root (/) partition. Select free space -> Add GPT partition. Enter the partition size, filesystem type (E.g. EXT4), and the mount point (E.g. /) and select "Create" and press ENTER. I have assigned the remaining space to the root partition.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/46a7ccac-f6f3-4be4-86c2-7545ce62bfe8)


After creating all required partitions, review the disk partition layout. If you are satisfied with current partitioning layout, choose "Done" and hit ENTER to save the changes.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/08b367ff-2ae4-41a8-9ba1-426d1ce200c9)

All the data in the disk will be deleted now. Please ensure there is no data in the drive and choose "Continue" to format the disk partitions.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0010b6cb-7f2c-4ff5-99af-9987e369bf36)

Step 10 - Enter Ubuntu Hostname and Username Information
In this section, enter the suitable hostname for your Ubuntu server. And also enter username and password that you will use to log in to your Ubuntu server.


![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/20044143-1e8e-459d-bbff-def9f9c255d5)


Step 11 - Enable Ubuntu Pro
If you have Ubuntu pro account, you can choose "Enable Ubuntu Pro" option. It will upgrade your Ubuntu server to get security updates until 2032.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0010b6cb-7f2c-4ff5-99af-9987e369bf36)


I don't have Ubuntu Pro account, so I skipped this it. You can register with Ubuntu Pro at any time later by entering the following command:

$ sudo pro attach

Step 12 - Configure SSH
In step, you can setup SSH. Check the "Install OpenSSH Server" check-box and choose "Done" and hit ENTER.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0010b6cb-7f2c-4ff5-99af-9987e369bf36)

Step 13 - Select Featured Server Snaps
In the next section, you will be presented with some popular snaps that you may want to install. Choose the snap applications of your choice and hit ENTER to continue. You can select or deselect the apps with the SPACEBAR key.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0010b6cb-7f2c-4ff5-99af-9987e369bf36)

Now the Ubuntu server installation will start. This will download and install a lots of packages. So please be patient.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0010b6cb-7f2c-4ff5-99af-9987e369bf36)

Step 14 - Reboot Ubuntu Server
Once the Ubuntu server installation is completed, select "Reboot Now" option and hit ENTER to reboot your Ubuntu server.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0010b6cb-7f2c-4ff5-99af-9987e369bf36)

Congratulations! Ubuntu 22.04 LTS server is successfully installed!

Log in to Ubuntu Server
Log in to your newly installed Ubuntu server. Enter the username and its password which you created during the installation process.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0010b6cb-7f2c-4ff5-99af-9987e369bf36)

Start using your newly installed Ubuntu 22.04 LTS server edition.

Update Ubuntu
The first thing after installing any OS is to update it. Ubuntu is no exception. Let us update the Ubuntu server by entering the following commands:

$ sudo apt update

$ sudo apt full-upgrade


![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0010b6cb-7f2c-4ff5-99af-9987e369bf36)


During the installing updates task, you will be prompted to restart some services. Choose OK to do so.

![image](https://github.com/Sankartridots/How-To-Install-Ubuntu-22.04-LTS-Server-Edition/assets/129372497/0ffa5478-6f96-44ce-8d93-6a64c34ecd07)

After all updates are applied, remove any leftover, unnecessary packages by running the following commands:

$ sudo apt autoremove

$ sudo apt autoclean

Finally, once again reboot your system.

$ sudo reboot


Conclusion
In this step by step tutorial, we learned how to download latest Ubuntu 22.04 LTS server version and how to create a Ubuntu bootable USB drive using the ISO and finally how to install Ubuntu 22.04 LTS server edition with screenshots.
