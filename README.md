# Ansible_BigIP
Ansible BigIP playbooks

# This playbook will provision the LTM Nodes, pools and Virtual servers sing the inputs from the var file.
# Its route domain and partition aware

This playbook will perform the below plays.

1. Identify the active and standby appliances.
2. Identify the sync-failover group.
3. Create the the new partition and sync to group.
4. Create new VLANs and SelfIps and Floating IPs.
5. Create nodes, Pools and virtual servers
6. Once all the resources are created make the final sync from the activive device to group.


## ansible-playbook -i hosts f5_provisioning.yml
