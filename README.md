# Configuration Management Project

Automate Linux server setup using **Ansible**.
https://github.com/haritt04/ansible-roles

## Overview
Learn configuration management by creating an Ansible playbook to:

- Set up a base system (updates, utilities, security)
- Install and configure **NGINX**
- Deploy a static website
- Add SSH keys for server access

## Getting Started

1. Prepare a Linux server and install Ansible locally.
2. Configure your `inventory.ini`.
3. Run the playbook:

```bash
ansible-playbook -i inventory.ini setup.yml
```

Run specific roles with tags:

```bash
ansible-playbook -i inventory.ini setup.yml --tags "nginx"

```
## Project Structure
```bash
setup.yml
inventory.ini
roles/
  ├── base
  ├── nginx
  ├── app
  └── ssh
```
