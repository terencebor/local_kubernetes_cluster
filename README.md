
These files can be used to create a Kubernetes kubeadm cluster on your local machine.
Cluster consists of one master and two worker nodes based on CentOS 7 (bento/centos-7).
For creation these Ansible playbooks used information from: https://kubernetes.io/docs/setup/independent/install-kubeadm/

Host system must have installed:
- Ansible (https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- Vagrant (https://www.vagrantup.com/intro/getting-started/install.html)
- Virtualbox (https://www.virtualbox.org/manual/ch01.html)

To start a cluster:
1. Create a project directory.
2. Copy files into the project directory.
3. Go into the project directory.
4. Run a command as a regular user: $ vagrant up
5. Wait until vagrant finished creating virtual machines (VM).
6. To check created VMs: $ vagrant status
7. ssh into master node: $ vagrant ssh master
8. ssh into worker node 1: $ vagrant ssh node01
9. ssh into worker node 2: $ vagrant ssh node02

User/password for all the VMs: vagrant/vagrant

Created and tested on Fedora 29 on Intel i5-6400 CPU with 12GB RAM
