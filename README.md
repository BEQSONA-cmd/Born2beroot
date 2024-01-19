# Born2beroot
42_Courses : Born2beroot (125%)
# STEP 1 configure debian

start with new VM:
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.23.54 PM-1.png>)

name should be : "Born2beroot"
and for my example i choose Oracle (64bit) for linux version
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.27.28 PM.png>) 

1GB RAM is enough for this VM
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.28.08 PM.png>) 

here create a virtual hard disk
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.28.58 PM.png>) 

VDI cuz we have ISO file
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.29.15 PM.png>) 

here we have to choose memory for allocate
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.29.33 PM.png>) 

i put 30.8 cuz im doin bonus, and click "Create"
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.30.03 PM.png>) 

go to "settings"
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.30.32 PM.png>) 

"Storage" below Controller: IDE is "Empty"
and in Optical Drive: choose a duisk file.
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.31.32 PM.png>) 

search ISO file for your VM and click "Open"
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.32.23 PM.png>) 

start your VM
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.32.48 PM.png>) 


# STEP 2 install Debian

go to "install" and follow the pictures
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.36.27 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 1.37.44 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 1.38.17 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 1.38.30 PM.png>) 

Hostname should be your intra name + 42 for example "btvildia42"
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.39.32 PM.png>) 

there is no specific reason to put Domain name, so i just left it empty
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.39.47 PM.png>) 

for your root password , you must to follow the "strong password policy"
and create strong password
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.42.16 PM.png>) 

i choose to put intra name here
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.42.45 PM.png>) 

and same here :)
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.43.42 PM.png>) 

for the password for my user i choose same as my root password
cuz i have small creativity :)
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.44.58 PM.png>)

go to manual for setting partitions in manual way,
its partition structure for bonus
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.47.58 PM.png>) 

choose our VBOX HARDDISK
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.48.33 PM.png>) 

Create new epmty partition table
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.48.46 PM.png>) 

choose our FREE SPACE
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.49.32 PM.png>) 

and create a first new partition
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.49.43 PM.png>) 

as we have in subject for example it should be:
500m Primary partition for Boot
so follow the steps 
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.57.49 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 1.58.03 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 1.58.15 PM.png>) 

Mout point should be Boot
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.59.13 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 1.59.27 PM.png>) 

click done setting up the partition and with that we create our first partition :)
![Alt text](<Photos/Screen Shot 2024-01-15 at 1.59.45 PM.png>) 

now click your FREE SPACE and create other Logical partition
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.00.33 PM.png>)

follow steps
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.01.03 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 2.01.39 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 2.02.53 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 2.03.20 PM.png>) 

here choose "Do Not Mount it"
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.03.44 PM.png>) 

![Alt text](<Photos/Screen Shot 2024-01-15 at 2.04.17 PM.png>) 

now we configure encrypted volumes on this partition
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.04.29 PM.png>) 


![Alt text](<Photos/Screen Shot 2024-01-15 at 2.04.44 PM.png>)


![Alt text](<Photos/Screen Shot 2024-01-15 at 2.05.02 PM.png>)

for use "arrows" for moves, for checking click "space" check sda5 and press "Enter"
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.05.19 PM.png>) 

click done setting up partition here
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.06.28 PM.png>) 

here finish
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.06.50 PM.png>) 

and here choose yes
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.07.02 PM.png>) 

you can skip this and press cancel
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.07.38 PM.png>) 

for the reason of zero creativity i put same password here :)
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.08.27 PM.png>) 

now we gonna start to configure LVM Groop (Logical Volume Manager)
wich should be like this (from subject)
![Alt text](<Photos/Screen Shot 2024-01-17 at 1.09.35 PM.png>)

so follow steps carefully 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.09.38 PM.png>)

![Alt text](<Photos/Screen Shot 2024-01-15 at 2.10.01 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.10.35 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.11.05 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.11.59 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.12.12 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.12.48 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.13.11 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.13.45 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.14.42 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.14.54 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.15.36 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.15.54 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.17.48 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.18.02 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.18.32 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.18.51 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.19.07 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.19.19 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.19.42 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.19.58 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.20.11 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.20.25 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.21.41 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.21.57 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.22.07 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.22.15 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.22.56 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.23.07 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.25.07 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.25.15 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.26.17 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.26.31 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.26.45 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.30.31 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.31.55 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.32.12 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.32.34 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.33.25 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.33.38 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.35.06 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.35.27 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.35.37 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.35.48 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.36.09 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.36.20 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.37.00 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.37.41 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.37.55 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.38.13 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.38.27 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.38.36 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.38.51 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.39.03 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.39.25 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.39.53 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.40.16 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.40.26 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.41.05 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.41.26 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.41.46 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.42.09 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.42.31 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.42.57 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.43.12 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.44.22 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.44.37 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.45.05 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.45.15 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.59.20 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.59.37 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 2.59.46 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 3.00.00 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 3.04.43 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 3.06.18 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 3.08.12 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 3.08.27 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 3.16.56 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 3.18.20 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 3.19.45 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 4.04.08 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 4.05.59 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 4.19.27 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 4.24.25 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 4.36.25 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 4.43.13 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 4.50.52 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 4.58.50 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.03.39 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.08.16 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.09.34 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.16.15 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.24.20 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.25.36 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.26.46 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.32.00 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.38.38 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.40.19 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.41.55 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.43.15 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.46.29 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 5.49.58 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 6.20.33 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 6.23.23 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 6.26.26 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 6.32.48 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 7.00.29 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 7.01.35 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-15 at 7.13.59 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.00.39 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.01.09 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.01.53 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.03.53 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.08.59 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.09.11 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.09.22 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.09.33 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.09.45 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.09.55 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.15.23 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.19.22 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.21.33 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.24.17 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.32.11 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.33.40 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.36.08 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.38.39 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.39.25 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 1.40.09 PM.png>) 
![Alt text](<Photos/Screen Shot 2024-01-16 at 3.03.49 PM.png>) 


