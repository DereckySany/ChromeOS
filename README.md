# ChromeOS
Chrome OS Easy Installation Scripts
1) Is this the same as Neverware Cloudready, Flint OS, Bliss OS or FydeOS ?
No its not, Its full fledged Official Chrome OS including Android Apps, Linux, Google Assistant, Chrome Sync which is not available usually in this releases. 

2) I'm stuck on google logo.
Your recovery image file may be corrupted. So re download it and follow the procedure again.

3) My hard drive has name different than sda.
You can edit the install.sh script and replace "sda" to your hdd name.
or enter the following commands line by line in terminal and replace your hdd name with "sdX"

sudo apt update
sudo apt install pv
sudo apt install cgpt
sudo chromeos-install.sh -src rammus_recovery.bin -dst /dev/sdX   

4) I am not able to boot up.
Please check your bios settings and disable secure boot, CSM, Legecy mode & turn on UEFI Boot option

5) I want to dual boot Chrome OS with Windows 10.
Please let me know in the comments down below so I can make a separate video for dual booting chrome os with windows 10.

6) ERROR  "cgpt needs to be installed first"
Make sure you are connected to the internet first before running installation script.

7) Linux apps (crostini) are not working at all, how do i fix it?
Go check if you have enabled all virtualization related option in your BIOS (Ex: "Intel Virtualization", "VT-x", "VT-e" etc...) (you should)

8)Do i need to install android on pc seperetely ?
No Official Chrome OS comes with android x86 so you don't need any android emulation software anymore.

9) I have non Intel based CPU. Can I install it?
No as of now non Intel based CPU's are not supported
