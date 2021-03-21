# Configuring Hadoop using Ansible and starting services.

#### The `masterconf.yml` file is used to configure master node of hadoop.
#### And `slaveconf.yml` file is used to configure slave node of hadoop.

`d_core-site.xml` and `d_hdfs-site.xml` files are the configuration files for slave node. We will copy both of these files to slave node at following location 
> /etc/hadoop
and save them with `core-site.xml` and `hdfs-site.xml` names respectively. These conf files contains all neccessary information to keep slave node up and running.

#### Similarly,
`n_core-site.xml` and `n_hdfs-site.xml` files, we will store at same location with same names respectively as we did in slave node, but only difference is that 
we will store it in master node.

#### Finally `hadoop-vars.yml` file contains all the variables that we used in `masterconf.yml` and `slaveconf.yml` files.

### If you want to implement this than you have to download all these files in your ansible manage node (one where you have setup ansible) in same folder or location. Also for hadoop we need hadoop rpm file and java rpm file. So download that also.
