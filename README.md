# Hard-Disk-Expansion
Hard Disk Expansion on VCenter

Get the host details and volume name.
Connect to the V-center on which the server is located. 
Once the VM is located on V-Center, the SCSI ID of the VM is calculated. 
Based on SCSI ID, the hard disk name is found which is supposed to be expanded.
To check availability of disk space, the datastore free space is checked. If the free space is more than 20%, then the control proceeds to next step, else an email is sent to Windows Team along with the ticket.
Based on the current Hard Disk capacity, the new HD capacity is calculated. The value is 20% higher than the older capacity. 
Hard Disk is set to the new value calculated in the previous step.
After this, log into the virtual machine to extend the disk drive on OS level.
It scans for the new disks for the volume and extends the disk on OS level.
Upon this, the task is complete.
