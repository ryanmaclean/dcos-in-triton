# OpenDCOS in Triton
Collection of Terraform configuration files and Ansible playbooks for setting up
OpenDCOS in Triton.

# Requirements
  * [Ansible](https://www.ansible.com) (`>= 2.0.0.2`)
  * [Terraform](https://www.terraform.io/) (`>= 0.6.14`)

# Development
Make sure that you have the following tools installed in your local environment:

  * [Vagrant](https://www.vagrantup.com) (`>= 1.8.1`)
  * [GNU Make](https://gnu.org/software/make/) (`>= 4.1`) (optional)

## Testing locally
You can simply run
```
make
```
This will bring up the Vagrant box and run the Ansible playbooks against it.

You can also do this all manually but the Makefile should help boosting your development
environment.

### Creating the Vagrant box
```
make vagrant
```

### Provisioning the Vagrant box with Ansible
```
make provision
```

### Destroying the Vagrant box
```
make destroy
```
