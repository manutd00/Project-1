# Project-1
## Automated ELK Stack Deployment
This is what I used to configure my ELK network.
![Network Diagram](https://github.com/manutd00/Project-1/blob/main/resources/Azure.png)

In this project I configured an ELK stack server in order to set up a cloud monitoring system.

  - [Ansible Files](https://github.com/manutd00/Project-1/tree/main/Ansible_Files)

This document contains the following details:
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

| Name     | Function | IP Address | Operating System |
|----------|----------|------------|------------------|
| Jump Box | Gateway  | 10.0.0.1   |       Linux      |
| Web 1    |Web server| 10.0.0.11  |       Linux      |
| Web 2    |Web server| 10.0.0.12  |       Linux      |
| Web 3    |Web server| 10.0.0.13  |       Linux      |
| VM ELK   |Web server| 10.1.0.4   |       Linux      |

### Access Policies
The machines on the internal network are not exposed to the public internet.
Only The Elk machine can accept connections from the internet. 

### Elk Configuration
Ansible was used to automate configuration of the ELK machine. No configuration was performed manually, which is advantageous because it alows you to effeciently use your apps. Ansible will get your systems running when you write a playbook.

The playbook implements the following tasks:
- Sets ELK stack together
- Monitors the servers

Command to excute PLaybook:
- sudo ansible-playbook site.yml

### Beats in Use
This ELK server is configured to monitor the following machines: 
- Web 1
- Web 2

I have installed the following beats on these machines: 
- ELK Server
- Web 1
- Web 2

These beats allowed me to collect information from each machine

### Using the Playbook
In order to use the playbook, you will need to have an Ansible control node already configured. Assuming you have such a node provisioned:

SSH into the control node and follow the steps below:
- Copy the ansible file to the virtual machine
- Update the /etc/ansible/hosts file to include the Ip addresses
- Run the playbook, and navigate to Kibana to check that the installation worked as expected.
