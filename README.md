# Tenant1 Org Config

This repository contains the configuration of a tenant in Ansible Automation Platform. The tenant is the owner of this repository, and they should store all configuration changes for their organization in this repo. This includes

- Credentials
- Credential Types
- Project
- Inventories
- Inventory sources
- Job Templates
- Workflow Templates

All configuration objects should be added to the inventory. See [inventory](inventory/group_vars/all/job_templates.yaml) for an example.

The configuration is applied via the [org-config](playbooks/org-config.yaml) playbook.

## Dependencies

This repository depends on the following Ansible collections:

- _ansible.platform_
- _ansible.controller_
- _ansible.hub_
- _ansible.eda_
- _infra.app_configuration_ 