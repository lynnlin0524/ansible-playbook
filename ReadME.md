## Prerequisites

- Ansible installed on the control machine.
- Target hosts accessible from the control machine.
- Sufficient privileges on the target hosts to install packages and start services.


## Install Ansible

1. Install Ansible on the control machine by following the instructions provided in the [Ansible documentation](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

2. Verify the installation by running the following command in your terminal:

   ```bash
   ansible --version


# Ansible Playbook: Install Docker 
This Ansible playbook automates the installation of Docker on VMs. It will update the package cache, install Docker, and start the Docker service.


## Usage

1. Clone this repository to your control machine or download the playbook and inventory files.

2. Edit the `inventory.ini` inventory file and replace `<public_ip_vm1>` and `<public_ip_vm2>` with the public IP addresses of your Azure VMs.

3. Adjust the variables in the `install-docker-playbook-ubuntu.yaml` playbook file if needed. 

4. Open a terminal and navigate to the directory containing the playbook and inventory files.

5. Run the following command to execute the Ansible playbook:

   ```shell
   ansible-playbook -i inventory.ini install-docker-playbook-ubuntu.yaml
