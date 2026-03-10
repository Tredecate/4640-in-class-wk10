# 4640-ansible-roles-lab

## Overview
This repository contains a refactored Ansible configuration that provisions two AWS EC2 instances created via Terraform. The original configuration is modularized into two distinct roles:

- **frontend**: Installs and configures an NGINX web server on Debian instnace serving a custom HTML template.
- **redis**: Installs a Redis Server on a Rocky Linux instance.

## Ansible Commands

**_NOTE_**: Need to install python3 botocore and boto3 to run the playbook successfully.

- `ansible-lint .`:The command checks the Ansible playbook for best practices and potential issues
- `ansible-playbook -i inventory playbook.yml`: The command runs the Ansible playbook using the specified inventory file.


- `ansible-inventory --graph`: The command displays the inventory in a graph format, showing the relationships between hosts and groups.

- `ansible all -m ping`: The command tests the connectivity of all hosts in the inventory.

