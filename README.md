Proxmox: Nested Virtualization
==============================

An Ansible role that enables nested virtualization on a Proxmox host.

Requirements
------------

N/A

Role Variables
--------------

|              Variable              |  Type  |                          Description                          |
| :--------------------------------: | :----: | :-----------------------------------------------------------: |
| `proxmox_nested_virt_cpu_override` | string | Override the auto-detected CPU manufacturer: `intel` or `amd` |

Dependencies
------------

N/A

Example Playbook
----------------

``` yaml
---
- name: Enable nested virtualization on all PVE nodes
  hosts: pve
  remote_user: root

  roles:
    - role: mirceanton.proxmox_nested_virt
      vars:
        proxmox_nested_virt_cpu_override: intel
```

License
-------

MIT

Author Information
------------------

A role developed by [Mircea-Pavel ANTON](https://www.mirceanton.com).
