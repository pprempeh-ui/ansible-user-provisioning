# Ansible User Provisioning Automation

## Overview

This project automates Linux user account provisioning using Ansible. It securely manages credentials with Ansible Vault and deploys SSH public keys for passwordless authentication.

## Features

* Automated user creation
* Group assignment
* SSH public key deployment
* Encrypted password management with Ansible Vault
* Idempotent automation

## Technologies

* Ansible
* YAML
* Linux (Rocky Linux / RHEL)
* SSH

## Project Structure

* `create_users.yml` - Main automation playbook
* `inventory` - Managed hosts inventory
* `public_keys/` - SSH public keys
* `ansible.cfg` - Ansible configuration

## How to Run

```bash
ansible-playbook -i inventory create_users.yml --ask-vault-pass
```
