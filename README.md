# Projet Netmonitoring

## Description
Ce projet vise à automatiser différentes tâches liées à la supervision réseau et à la gestion des serveurs au sein d'une infrastructure. En utilisant Ansible, nous automatisons l'installation et la configuration du service SNMP sur les machines Linux et Windows, ainsi que l'ajout de ces machines à la supervision via Centreon. De plus, nous gérons de manière automatisée la génération et l'affectation de mots de passe sur les systèmes Linux et Windows.

## Objectifs
- Automatiser l'installation et la configuration du service SNMP sur Linux et Windows.
- Automatiser l'ajout des machines Linux et Windows à la supervision via Centreon.
- Automatiser la gestion des mots de passe sur les systèmes Linux et Windows.

## Description des Playbooks

1. **[Inventory.yml](https://github.com/Sushitsu/ansible-project/blob/master/Inventory/inventory.yml)**
    - Crée un inventaire des machines à superviser.

2. **[add_snmp_linux.yml](https://github.com/sushitsu/ansible-project/Playbooks/add_snmp_linux.yml)**
    - Automatise l'installation et la configuration du service SNMP sur les machines Linux.

3. **[remove_snmp_linux.yml](https://github.com/sushitsu/ansible-project/Playbooks/remove_snmp_linux.yml)**
    - Automatise la suppression du service SNMP des machines Linux.

4. **[password_management_linux.yml](https://github.com/sushitsu/ansible-project/Playbooks/password_management_linux.yml)**
    - Génère et affecte de manière aléatoire un mot de passe sur les systèmes Linux.

5. **[add_snmp_windows.yml](https://github.com/sushitsu/ansible-project/Playbooks/add_snmp_windows.yml)**
    - Automatise l'installation et la configuration du service SNMP sur les machines Windows.

6. **[remove_snmp_windows.yml](https://github.com/sushitsu/ansible-project/Playbooks/remove_snmp_windows.yml)**
    - Automatise la suppression du service SNMP des machines Windows.

7. **[password_management_windows.yml](https://github.com/sushitsu/ansible-project/Playbooks/password_management_windows.yml)**
    - Génère et affecte de manière aléatoire un mot de passe sur les systèmes Windows.

8. **[add_hosts.yml](https://github.com/sushitsu/ansible-project/Playbooks/add_hosts.yml)**
    - Automatise l'ajout des hôtes à Centreon pour la supervision.

9. **[remove_hosts.yml](https://github.com/sushitsu/ansible-project/Playbooks/remove_hosts.yml)**
    - Automatise la suppression des hôtes de Centreon.

## Commandes pour exécuter les Playbooks

- Pour exécuter un playbook Ansible, utilisez la commande suivante :

  **ansible-playbook { inventory } { playbook }**

Assurez-vous d'avoir correctement configuré votre environnement Ansible avec les fichiers d'inventaire appropriés et les informations de connexion aux machines cibles avant d'exécuter les playbooks.
