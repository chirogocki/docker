# Ansible roles to manage cluster

## Prepare for swarm

### Init role

This role ensure minimal packages on host, copy bashrc and mount necessary NFS share for the **swarm**.
Two variables are important :

| Variable | Usage |
|----------|:---------:|
| dietpi_home_path | **Dietpi** user data can be stored locally or over NFS. This path contains **docker data** |
| docker_conf_path | NFS path where /config container and docker-compose are stored |

### Keepalived

Keepalived help accessing the swarm with a virtual IP. Each hosts participate as a node with two role master or backup.  
All config variables are in [inventory file](../inventories/README.md).  

### Docker

As **docker** package is installed/updated with **Dietpi** distribution this Ansible role only tune OS limits.  

### Check - Reboot - Shutdown

Collection of utilities aka "SwissKnife".  
Check role send slack notifications on hosts status.  

### Swarm

Automate **docker swarm** creation with three usage type :
* manager1 : the first manager node (whom initiate the swarm)
* managers : managers nodes
* workers : workers nodes

### Swarm-network
