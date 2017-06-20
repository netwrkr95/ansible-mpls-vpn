# ansible-ios-xe
Work in progress for generating Ansible playbooks for common and more complex IOS-XE configurations in Cisco routers and switches.  The focus of these early playbooks are targeting automating the configuration of creating new VRF's into IOS-XE, specifically a Cisco CSR.  The ability to leverage Ansible playbooks for any "global" configuration commands within IOS-XE or any router or switch configuration, could be quite appealing to operators.

In these basic playbook examples, the VRF parameters required are entered as variables directly into the playbook, under "vars".  This allows any operator to use those 5 parameters to create minimal VRF configurations on an IOS-XE device.

The other playbook included here, will support any "show commands" for an IOS-XE device, using the "-e" options on the command line when executing an Ansible playbook.  This can be very useful and keep the configuration simple for the operator, executing any known "show" command from the same prompt that is executing the playbooks.
