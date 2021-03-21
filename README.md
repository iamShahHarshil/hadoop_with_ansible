# Configuring Hadoop using Ansible and starting services.

#### The `masterconf.yml` file is used to configure master node of hadoop.
#### And `slaveconf.yml` file is used to configure slave node of hadoop.

`d_core-site.xml` and `d_hdfs-site.xml` files are the configuration files for slave node. We will copy both of these files to slave node at following location 
> /etc/hadoop
and save them with `core-site.xml` and `hdfs-site.xml` names respectively. These conf files contains all neccessary information to keep slave node up and running.

#### Similarly,
`n_core-site.xml` and `n_hdfs-site.xml` files, we will store at same location with same names respectively as we did in slave node, but only difference is that 
we will store it in master node.
