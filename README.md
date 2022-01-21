# Project-1
## Automated ELK Stack Deployment
This is what I used to configure my ELK network.
![Network Diagram](https://github.com/manutd00/Project-1/blob/main/resources/Azure.png)

(short description of project)

  - [Ansible Files](https://github.com/manutd00/Project-1/tree/main/Ansible_Files)

The document contains the following details:
- Description of the Topology
- Access Policies
- Elk Configuration
-   Beats in Use
-   Machines Being Monitored
- Using the Playbook

### Description of the Topology
 This network exposes a load-balanced and monitored instance of DVWA.
 
 Load balancing restricts access to the network and will be highly effecient by spreading the work evenly. 
 - Load balancers protect against emerging threats
 - The jump box alows us top open one oprt to the VM instead of many
 - Layer of security, prevents exposure to public
 
 Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the data and system logs
 - Filebeat is used to monitor log files
 - Metricbeat moves information to specified output


The configuration details of each machine may be found below.



### Access Policies
The machines on the internal network are not exposed to the public internet.


### Elk Configuration


### Beats in Use


### Using the Playbook
