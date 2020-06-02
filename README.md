# Hard-Disk-Expansion
Hard Disk Expansion on VCenter

1. Get the host details and volume name.
2. Connect to the V-center on which the server is located. 
3. Once the VM is located on V-Center, the SCSI ID of the VM is calculated. 
4. Based on SCSI ID, the hard disk name is found which is supposed to be expanded.
5. To check availability of disk space, the datastore free space is checked. If the free space is more than 20%, then the control proceeds to next step.
6. Based on the current Hard Disk capacity, the new HD capacity is calculated. The value is 20% higher than the older capacity. 
7. Hard Disk is set to the new value calculated in the previous step.
8. After this, log into the virtual machine to extend the disk drive on OS level.
9. It scans for the new disks for the volume and extends the disk on OS level.
10. Upon this, the task is complete.
