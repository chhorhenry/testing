\*The version of Clonezilla the team uses is 2.7.1-22 amd64, please use the same version by downloading the iso file from the link below\* 

[https://osdn.net/projects/clonezilla/downloads/74519/clonezilla-live-2.7.1-22-amd64.iso/ ](https://osdn.net/projects/clonezilla/downloads/74519/clonezilla-live-2.7.1-22-amd64.iso/) Afterwards, turn the iso into a bootable drive depending on what OS you are on. 

- Windows 
  - Download Rufus from[ https://rufus.ie/en_US/ ](https://rufus.ie/en_US/) 
  - Insert your USB into the machine 
  - Open Rufus and use the tool to turn the USB into a bootable clonezilla drive 
- Linux 
- sudo add-apt-repository ppa:gezakovacs/ppa  
- sudo apt-get update  
- sudo apt-get install unetbootin 
- Insert USB into machine 
- Open Unetbootin 
- Click into lower half and select the iso you downloaded 

\*After the drive is complete, restart machine and press F9 to get to boot menu, and select the drive\* 

- After Clonezilla boots up 
- Select VGA default settings 
- Select English 
- Keep the default keyboard 
- Start Clonezilla 
- Device-image 
- Local dev is you are using the usb drive as the storage 
  - From here everything is fairly straightforward as you are locked into certain selections 
  - Only crucial thing is selecting the drive you want to clone, make sure it is the proper one, and good naming convention is advised 
- Select ssh-server if you are trying to send or retrieve one of the images on the lab network 
  - After connecting, enter this information: 
    - IP Address: 192.168.1.26 
    - Root: 22 
    - User: DSADMIN 
    - Password: allseeing 
  - From here, the directory you want to access is: 
- /mnt/md0/sharedata/images/[fill] 
- The fill will be one of the following 
- Test-Test images or if Henry puts one there specifically for you 
- Production-Images that are currently in production 
- Archive-Images from the past that have been phased out 

\*That is it! You are welcome to clone any images from the directories, but if you are adding one, please let Henry Chhor know at[ henry.chhor@hp.com ](mailto:henry.chhor@hp.com)so he can make it executable\* 
