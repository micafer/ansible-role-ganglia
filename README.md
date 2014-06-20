Ganglia ansible role
=========================

Installs and configure Ganglia monitoring system in a cluster of nodes.
How to use it:

In the "Monitored nodes"
```yml
 roles: 
    - { role: 'ganglia',  ganglia_gmetad: 'MASTER_NODE_NAME_OR_IPr' }
```

In the "Ganglia meta Daemon node"
```yml
 roles: 
    - { role: 'ganglia', ganglia_gmetad: 'MASTER_NODE_NAME_OR_IP', ganglia_type_of_node: 'master'}
```

