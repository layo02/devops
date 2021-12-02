Run this playbook (site.yml)
1. Fill up the `hosts` file with desired manager and worker node ip-addresses.
2. Install `atosatto.docker-swarm` playbook via ansible-galaxy. `ansible-galaxy install atosatto.docker-swarm`
3. run `ansible-playbook -i hosts -K site.yml --extra-vars "python_pip_packages=python3-pip"`
4. For local testing (for example via Vagrant VM) recommended to add to extra-vars one more parameter `docker_swarm_interface=eth1` for specifing external network interface for VMs.
 
 Run monitoring playbook (master.yml)
1. Enter directory `ansible_playbook`
2. Make sure that the group `[docker_swarm_monitoring_endpoint]` contains the endpoint hostname
3. Run `ansible-playbook -i docker_swarm_cluster/hosts -u <username> master.yml -K`