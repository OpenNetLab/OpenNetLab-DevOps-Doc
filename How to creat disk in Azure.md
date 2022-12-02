# How to creat disk in Azure

Step 1, select the virtual machine that you want to add in the resource list 
![image](https://github.com/wangyf2001/Azure-picture/blob/main/image1.png)

Step 2, click on the Disk options  
![](https://github.com/wangyf2001/Azure-picture/blob/main/image2.png)

Step 3, select a new hard disk in the data disk 
![](https://github.com/wangyf2001/Azure-picture/blob/main/image3.png)

Step 4, fill in the disk size and other content according to your own needs 
![](https://github.com/wangyf2001/Azure-picture/blob/main/image4.png)

Step 5, click Save 
![](https://github.com/wangyf2001/Azure-picture/blob/main/image5.png)

Step 6, add it successfully 
![](https://github.com/wangyf2001/Azure-picture/blob/main/image6.png)

Step 7: Formatting the disk
Use the fdisk-l command to view the disk   
![](https://github.com/wangyf2001/Azure-picture/blob/main/image7.png)

Step 8: Format the hard disk file system

> mkfs -t ext4 /dev/sdc

Step 9, Mount the hard drive

Create a directory that you want to mount

> mkdir /onldata

Mount the hard disk to the folder

> mount /dev/sdc /onldata

Step 10, boot on automatic mount

> vim /etc/fstab  
![](https://github.com/wangyf2001/Azure-picture/blob/main/image8.png)
