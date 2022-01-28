Ansible playbook for EFK stack deployment

Example usage:
> ansible-playbook -u <remote-user-name> -e inventories/dev/group_vars/efk.yml -i inventories/dev/inventory.is2.dev master.yml -K
