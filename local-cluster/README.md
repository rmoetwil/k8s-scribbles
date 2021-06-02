# Local Cluster setup using vagrant and ansible

Setting up your local k8s cluster with vagrant and ansible.
Based on instructions found [here](https://kubernetes.io/blog/2019/03/15/kubernetes-setup-using-ansible-and-vagrant/).

Prerequisites:

- [Vagrant](https://www.vagrantup.com/)
- [Ansible](https://www.ansible.com/)
- [Virtual Box](https://www.virtualbox.org/)

## Local setup

From inside the folder `local-cluster`  run `vagrant up`.

The ansible playbooks found in the directory `kubernetes-setup` will be run automatically by Vagrant.

When ready you can ssh into the master via `vagrant ssh k8s-master` and into the nodes via `vagrant ssh node-[1-3]`.

Run `vagrant halt` to stop the VM's and `vagrant destroy` to remove all VM's that were created.
