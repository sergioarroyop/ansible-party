# ansible-party

# Setup
Install Ansible:
https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

To run a playbook, use the `ansible-playbook` command:

```
ansible-playbook
    -i <inventory> specify inventory host path or comma separated host list. –inventory-file is deprecated
    -m <module_name> module name to execute (default=command)
    -a <module_args> module arguments
    -b <become> run operations with become (does not imply password prompting)
    -v <verbose> verbose mode (-vvv for more, -vvvv to enable connection debugging)
```

To run vagrant.yml, for example:
```
ansible-playbook -i inventory/hosts_vagrant playbooks/vagrant.yml
```
