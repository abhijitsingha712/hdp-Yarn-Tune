hdp-yarn-tunning
=================

Ambari YARN UTILS.

To calculate the various parameters for YARN and MapReduce 2 use yarn-utils.py script. 

To find the parameters detaills use below commands ->>

To get core (c) information : 

      lscpu | grep -i core

To get memory(m) information : 

      free -h

To get disks(d) information : 

      lsblk
      
Require Python version 2.8 or less. 

      python2 yarn-utils --help for more info.


Example:

cd hdp-Yarn-Tune/scripts

python2 yarn-utils.py -c 16 -m 64 -d 4 -k True


by default the script uses the following:

cores = 16 (-c option)
memory = 64 (-m option)
disks = 4 (-d option)
hbaseEnabled (-k option)

