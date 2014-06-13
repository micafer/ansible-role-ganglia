Ganglia ansible role
=========================

Installs and configure Ganglia monitoring system in a cluster of nodes.
How to use it:

In the "Monitored nodes"
```yml
 roles: 
    - { role: 'ganglia',  ganglia_gmetad: 'master' }
```

In the "Ganglia meta Daemon node"
```yml
 roles: 
    - { role: 'ganglia', ganglia_gmetad: 'master', ganglia_type_of_node: 'master'}
```

