# Provisioning Ubuntu VMs with Apache2 and Bind9 using Ansible

This repository contains configuration files for provisioning Ubuntu VMs with Apache2 and Bind9 using Ansible. It includes a Vagrantfile for defining VM configurations and a playbook.yaml file for specifying Ansible tasks.

## Files

- `Vagrantfile`:
  The Vagrantfile defines the VM configurations using Vagrant. It sets up two Ubuntu 20.04 VMs named "satu" and "dua". The VMs are provisioned using Ansible by specifying the playbook to run.

- `playbook.yaml`:
  The playbook.yaml file contains Ansible tasks for provisioning the VMs. It updates the apt cache, installs Apache2 and Bind9, and enables their services.

## Usage

1. Ensure you have Vagrant and VirtualBox installed on your machine. You can download them from the following links:
   - [Vagrant](https://www.vagrantup.com/downloads)
   - [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

2. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/athallabf/vagrant-ansible.git
   ```

3. Navigate to the repository directory:

   ```bash
   cd vagrant-ansible
   ```

4. Modify the `Vagrantfile` if necessary, such as adjusting VM names or box versions.

5. Run the following command to start provisioning the VMs:

   ```bash
   vagrant up
   ```

6. Ansible will automatically run the playbook (`playbook.yaml`) to install Apache2 and Bind9 on the VMs.

7. Once provisioning is complete, you can access the VMs and verify the services are running as expected.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.


