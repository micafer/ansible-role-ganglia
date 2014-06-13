Ganglia ansible-playbooks
=========================

Installs and configure Ganglia monitoring system in a cluster of nodes.
How to use it:

In the "Monitored nodes"
```yml
 roles: 
    - { role: 'ganglia', ganglia_gmetad: 'master', ganglia_type_of_node: 'slave'}
```

In the "Ganglia meta Daemon node"
```yml
- include: ganglia/tasks/ganglia.yml is_client=no ganglia_gmetad=<MASTER_NODE_NAME_OR_IP>
```

