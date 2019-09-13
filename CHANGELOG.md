# v1.0.1
This is a minor release update of SimpliVity vra plugin. This release includes some key features that are listed below:
•	Support to delete Simplivity backup of a Virtual machine
•	Implemented vRA custom workflows to Set SimpliVity Backup Policy for the VM created using vRA blueprints
•	Option to power Off VMs in SimpliVity Move operation
•	Follow the SimpliVity tasks in all the workflows by eliminating any extra sleep or wait time

# v1.0.0
#### Notes
 This is the first release of the VRA plugin for simplivity. It adds full support to all the operations mentioned in the design guide.
 This version of the plugin supports the version of each product listed in the design guide and supports all subsequent versions until the document is
 replaced by a new edition.

#### HPE SimpliVity, the following functionalities are extended to vRA:
- Create and delete backup policy
- Set backup policy on a virtual machine or multi-machine service
- Backup and restore a virtual machine or multi-machine service
- Move a virtual machine or multi-machine service
- Clone a virtual machine
- Create, delete, and resize HPE SimpliVity datastore
- Display the list of backups and its sizes associated with a virtual machine
