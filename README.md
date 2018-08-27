open-vm-tools
=========

Installs and configures open-vm-tools for GUI environments.

Requirements
------------

None

Role Variables
--------------

Set `mount_hgfs` to `true` to use VMware's Shared Folders.

mount_hgfs: ""

Dependencies
------------

None

Example Playbook
----------------

Run playbook and mount HGFS share

```yml
  - hosts: servers
    roles:
        - { role: leesoh.open-vm-tools, mount_hgfs: true }
```

Alternatively, run the playbook with the `--extra-vars "mount_hgfs=true"` parameter.

License
-------

BSD
