# HPE SimpliVity plugin for VMware vRealize Automation

## Overview

The HPE SimpliVity hyperconverged infrastructure is designed from the ground up for today’s highly virtualized IT environments. The solution
eliminates cost and complexity by consolidating a variety of IT functions—including compute, storage, network switching, replication, and
backup—onto virtualized, industry-standard x86 hardware. Unlike legacy IT solutions based on monolithic data architectures, the HPE SimpliVity
hyperconverged infrastructure performs inline data deduplication, compression, and optimization on all data at inception across all phases of the
data lifecycle. By minimizing I/O and network traffic, routine operations such as application cloning, backup, and restore functions can be
completed in seconds or minutes instead of hours or even days.

## VMware® vRealize Automation
VMware vRealize Automation (vRA) streamlines the delivery and administration of private, public, and hybrid cloud applications and services.
The solution helps IT organizations accelerate service velocity, boost business agility, and contain operations expenses by automating IT service
deployment and lifecycle management tasks. Application developers and other users turn up compute resources and applications on-demand
without IT involvement, using self-service portals and service catalogs.

## HPE SimpliVity and vRA
HPE SimpliVity has fully integrated and rigorously tested HPE SimpliVity 380 with vRA, enabling HPE SimpliVity customers to fully experience
the features and benefits of VMware’s popular IT service delivery platform. The HPE SimpliVity hyperconverged infrastructure streamlines IT
operations and accelerates service velocity by unifying administrative tasks—all resources and features are centrally provisioned from the
VMware® vCenter™ management console. When integrated with vRA, HPE SimpliVity boosts business agility and improves IT operational
efficiencies even further by allowing users (application developers) to deploy and manage applications and compute services on their own. With
vRA, users can go online, request a new application or compute resource, and receive it in a matter of minutes, using simple service catalogs. The
integrated solution—HPE SimpliVity and VMware vRA—enables IT organizations to mobilize and protect virtualized workloads at scale. Users
can back up, restore, clone, and move their virtual machines on-demand via the vRA interface—all under strict administrative control of the
central IT organization.

## Design scenarios and considerations
Please check the Design guide for complete list of VRA design scenarios and considerations.
[Click here](https://github.com/HewlettPackard/simplivity-vra-plugin/blob/master/HPE%20SimpliVity%20with%20VMware%20vRealize%20Automation%20Design%20guide.pdf#page=5)

## Functionalities
The following functionalities are extended to vRA:
• Create and delete backup policy
• Set backup policy on a virtual machine or multi-machine service
• Backup and restore a virtual machine or multi-machine service
• Move a virtual machine or multi-machine service
• Clone a virtual machine
• Create, delete, and resize HPE SimpliVity datastore
• Display the list of backups and its sizes associated with a virtual machine

Please visit design guide for more details on each functionality.
[Click here](https://github.com/HewlettPackard/simplivity-vra-plugin/blob/master/HPE%20SimpliVity%20with%20VMware%20vRealize%20Automation%20Design%20guide.pdf#page=15)

Also please note: vRA Move Operation – Second vcenter is configured in both vRA and vRO. 
	• By adding to vRA, the cluster and storage details of the 2nd vcenter will be available after the MOVE operation
	• By adding to vRO, the subsequent Simplivity operations (after simplivity DC move) will be continue to work only if the 2nd vcenter is available in vRO.
Else vRO cannot process any simplivity request and an error will be visible in the vRA portal.

## Installation
The step by step guide to the installation is also documented in the design guide. Please visit the below link for the same.
[Click here](https://github.com/HewlettPackard/simplivity-vra-plugin/blob/master/HPE%20SimpliVity%20with%20VMware%20vRealize%20Automation%20Design%20guide.pdf#page=27)
