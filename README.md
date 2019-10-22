# Deploy latest ansible to debian

The default debian one is pretty old. Ironically Ansible [provide a list of instructions](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#latest-releases-via-apt-debian) for the latest version install, but no playbook!

## Example

```
---
- hosts: all
  become: yes
  roles:
    - {role: ./roles/ansible-role-deploy-ansible-latest}
```