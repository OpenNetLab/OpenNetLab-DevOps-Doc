# How To Create Disk In Azure

Step 1, select the virtual machine that you want to add in the resource list 

![image](./images/Azure/image1.png)

Step 2, click on the Disk options  

![](./images/Azure/image2.png)

Step 3, select a new hard disk in the data disk  

![](./images/Azure/image3.png)

Step 4, fill in the disk size and other content according to your own needs  

![](./images/Azure/image4.png)

Step 5, click Save  

![](./images/Azure/image5.png)

Step 6, add it successfully  

![](./images/Azure/image6.png)

Step 7, Formatting the disk

Use the fdisk-l command to view the disk  

![](./images/Azure/image7.png)

Step 8, Format the hard disk file system

> mkfs -t ext4 /dev/sdc

Step 9, Mount the hard drive

Create a directory that you want to mount

> mkdir /onldata

Mount the hard disk to the folder

> mount /dev/sdc /onldata

Step 10, boot on automatic mount

> vim /etc/fstab  

![](./images/Azure/image8.png)
