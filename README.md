# Automatic OS upgrade for Virtual Machine Scale Set. 
VMSSrollingupdate

Enabling automatic OS image upgrades on your scale set helps ease update management by safely and automatically upgrading the OS disk for all instances in the scale set.

Automatic OS upgrade has the following characteristics:

- Once configured, the latest OS image published by image publishers is automatically applied to the scale set without user intervention.
Upgrades batches of instances in a rolling manner each time a new image is published by the publisher.
- Integrates with application health probes and Application Health extension.
- Works for all VM sizes, and for both Windows and Linux images.
- You can opt out of automatic upgrades at any time (OS Upgrades can be initiated manually as well).
- The OS Disk of a VM is replaced with the new OS Disk created with latest image version. Configured extensions and custom data scripts are run, while persisted data disks are retained.
- Extension sequencing is supported.
- Automatic OS image upgrade can be enabled on a scale set of any size.


<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsabil05%2FVMSSUpdateRolling%2Fmaster%2Fnew_vmss.json" target="_blank">
    <img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.png"/>
</a>
