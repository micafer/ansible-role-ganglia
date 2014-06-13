Ganglia ansible-playbooks
=========================

Installs and configure Ganglia monitoring system in a cluster of nodes.
How to use it:

In the "Monitored nodes"
```yml
  vars_files: 
    - [ "utils/vars/{{ ansible_distribution }}.yml", "utils/vars/os_defaults.yml" ]

 roles: 
    - { role: 'ganglia',  ganglia_gmetad: 'master' }
```

In the "Ganglia meta Daemon node"
```yml
  vars_files: 
    - [ "utils/vars/{{ ansible_distribution }}.yml", "utils/vars/os_defaults.yml" ]

 roles: 
    - { role: 'ganglia', ganglia_gmetad: 'master', ganglia_type_of_node: 'master'}
```

