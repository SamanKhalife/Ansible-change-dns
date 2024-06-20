Role Name
=========

This role will help you to set new DNS servers IP for your hosts.

Requirements
------------

 Ansible 2.9 or higher

Role Variables
--------------

- `nameservers`: List of DNS server IP addresses. Default is `['8.8.8.8', '8.8.4.4']`.

Example Playbook
----------------

Include the role in Playbook

```
    - hosts: all
      become: true
      roles:
        - role: samankhalife.Changing-Dns
```
Note
-----
to change dns ips you can  change `defaults/main.yml`

or

just define it in your playbook

```
- hosts: all
  become: true
  roles:
    - role: samankhalife.Changing-Dns
      vars:
        nameservers:
          - 9.9.9.9
          - 149.112.112.112

```
Dependencies
------------

None

License
-------

MIT
