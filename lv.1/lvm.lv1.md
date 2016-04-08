```
############################################################ 
 
              LVM (logical volume management) 
                    HACK-SHEET LV.1 
############################################################ 
 
pvcreate /dev/sda2 = Creates a fisical volume in sda2 
pvdisplay = show the fisical volumes 
vgcreate VolGroup0 /dev/sda2 = creates a volume group called VolGroup0 in sda2 
vgextend VolGroup0 /dev/sdb1 = Extends the volume group to sdb1 
vgdisplay = show the volume groups 
lvcreate -L 10G VolGroup0 -n lvhome = creates a logical volume with a size of 10 giga named lvhome in VolGroup0 volume group (add -C y to swap partitions). You can use -l +100%FREE instead of -L 10G to use the entire avaiable space in disk. 
 
modprobe dm-mod = ups the device mapper kernel module needed to use lvm2. 
```