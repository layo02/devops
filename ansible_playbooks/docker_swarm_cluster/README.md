Run this playbook
1. Fill up the `hosts` file with desired manager and worker node ip-addresses.
2. Install `atosatto.docker-swarm` playbook via ansible-galaxy. `ansible-galaxy install atosatto.docker-swarm`
3. run `ansible-playbook -i hosts -K site.yml --extra-vars "python_pip_packages=python3-pip"`
4. For local testing (for example via Vagrant VM) recommended to add to extra-vars one more parameter `docker_swarm_interface=eth1` for specifing external network interface for VMs.
 