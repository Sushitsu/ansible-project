# Netmonitoring Project

## Description
This project aims to automate various tasks related to network monitoring and server management within an infrastructure. By using Ansible, we automate the installation and configuration of SNMP service on both Linux and Windows machines, as well as adding these machines to monitoring via Centreon. Additionally, we manage password generation and assignment on Linux and Windows systems in an automated manner.

## Objectives
- Automate the installation and configuration of SNMP service on Linux and Windows.
- Automate the addition of Linux and Windows machines to monitoring via Centreon.
- Automate password management on Linux and Windows systems.

## Playbooks Description

1. **[Inventory.yml](https://github.com/Sushitsu/ansible-project/blob/master/Inventory/inventory.yml)**
    - Creates an inventory of machines to monitor.

2. **[add_snmp_linux.yml](https://github.com/Sushitsu/ansible-project/tree/master/Playbooks/add_snmp_linux.yml)**
    - Automates the installation and configuration of SNMP service on Linux machines.

3. **[remove_snmp_linux.yml](https://github.com/Sushitsu/ansible-project/tree/master/Playbooks/remove_snmp_linux.yml)**
    - Automates the removal of SNMP service from Linux machines.

4. **[password_management_linux.yml](https://github.com/Sushitsu/ansible-project/tree/master/Playbooks/password_management_linux.yml)**
    - Generates and assigns passwords randomly on Linux systems.

5. **[add_snmp_windows.yml](https://github.com/Sushitsu/ansible-project/tree/master/Playbooks/add_snmp_windows.yml)**
    - Automates the installation and configuration of SNMP service on Windows machines.

6. **[remove_snmp_windows.yml](https://github.com/Sushitsu/ansible-project/tree/master/Playbooks/remove_snmp_windows.yml)**
    - Automates the removal of SNMP service from Windows machines.

7. **[password_management_windows.yml](https://github.com/Sushitsu/ansible-project/tree/master/Playbooks/password_management_windows.yml)**
    - Generates and assigns passwords randomly on Windows systems.

8. **[add_hosts.yml](https://github.com/Sushitsu/ansible-project/tree/master/Playbooks/add_hosts.yml)**
    - Automates the addition of hosts to Centreon for monitoring.

9. **[remove_hosts.yml](https://github.com/Sushitsu/ansible-project/tree/master/Playbooks/remove_hosts.yml)**
    - Automates the removal of hosts from Centreon.

## Commandes pour exécuter les Playbooks

- To execute an Ansible playbook, use the following command:

  **ansible-playbook { inventory } { playbook }**

Make sure you have correctly configured your Ansible environment with appropriate inventory files and connection information to target machines before running the playbooks.
