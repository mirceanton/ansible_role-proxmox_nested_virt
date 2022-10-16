Proxmox: Nested Virtualization
==============================

An Ansible role that enables nested virtualization on a Proxmox host.

Requirements
------------

N/A

Role Variables
--------------

|            Variable            |  Type  |   Default   |              Description               |
| :----------------------------: | :----: | :---------: | :------------------------------------: |
| `proxmox_nested_virt_cpu_type` | string | `UNDEFINED` | The CPU manufacturer: `intel` or `amd` |

Dependencies
------------

N/A

Example Playbook
----------------

``` yaml
---
- hosts: all
  remote_user: root

roles:
    - role: mirceanton.proxmox_nested_virt
      vars:
        proxmox_nested_virt_cpu_type: intel
```

License
-------

MIT

Author Information
------------------

A role developed by [Mircea-Pavel ANTON](https://www.mirceanton.com).
