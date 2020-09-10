# rhel8-iso-maker
Create individual RHEL8 ISOs for each node with static IPs

Variables can be defined in `group_vars/all.yml`

Define all the nodes you want an ISO created for in inventory.yml

To execute playbook, run the following command: `ansible-playbook playbook.yml -K`

ISOs will be created in the `/tmp` directory. The `-K` option is to request the BECOME password which is required to mount an ISO (assuming you don't have passwordless sudo).
