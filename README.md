# Installing wordpress with ansible

## Dependencies
![Badge](https://img.shields.io/badge/Ubuntu-18.04-red)
![Badge](https://img.shields.io/badge/ansible-2.9.10-blue)
![Badge](https://img.shields.io/badge/python-2.7.17-red)

# Edit inventory file

# To test host communication
```
ansible localhost -m ping
```

## Playbook example
```
---
- name: Install wordpress
  hosts: all
  become: yes
  roles:
  - server
  - php
  - mysql
  - wordpress
```
```
ansible-playbook -i hosts playbook.yml
```
## License
![Badge](https://img.shields.io/badge/license-GPLv3-green)

