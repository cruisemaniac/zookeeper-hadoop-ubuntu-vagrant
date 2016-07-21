# zookeeper-hadoop-ubuntu-vagrant
Ubuntu trusty64 based 8 vm setup with zookeeper and hadoop.

Sets up the following nodes:

Zookeeper - 3 nodes

Hadoop Namenodes - 2 nodes

Hadoop Datanodes - 3 nodes

#Steps to run:

1. ````vagrant up````
2. ````vagrant ssh-config```` - Get the port numbers from this list and update each node's port details in the ````dev_hosts```` file
3. Run ````ansible-playbook -i dev_hosts site.yml -vvvv```` to provision the machines.

#Caveats / Todo:

1. Configuration is default at the moment - No specific changes for any setup is done
2. NTP time update does not work yet ( Needs to be built in )
3. No workloads at the moment.
