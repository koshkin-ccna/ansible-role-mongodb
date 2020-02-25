mongodb
=========
Ansible Role - MongoDB

Requirements
------------
Role has been tested on CentOS 7.7 x86_64 with Ansible 2.9.4 and Python 3.7.6

Role Variables
--------------

MongoDB server is configured to listen all available interfaces, but you can change this behaviour by changing `bind` variable. Default `bind: 0.0.0.0`. You can also override default `port` and `path`.

Dependencies
------------

No dependent roles

Example Playbook
----------------

```yaml
---
 - hosts: vagrant-centos
   gather_facts: true
   become: true
   become_user: root
   become_method: sudo
   roles:
    - koshkin_ccna.ansible_role_mongodb
```

License
-------

MIT

Author Information
------------------

Credits to James Kiarie https://www.tecmint.com/author/james2030kiarie/ https://www.tecmint.com/install-mongodb-in-centos-8/ 