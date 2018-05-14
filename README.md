zabbix-templates-role
=====================

This role is to import templates into zabbix. Currently it is importing a single template, so the role will need to be extended to import multiple templates more efficiently.

It is an older solution to the issue and is no longer in active use.

Requirements
------------

None

Role Variables
--------------

`zabbix_url`: This is the zabbix api url
`zabbix_token`: Token to auth against the api

Dependencies
------------

None

Testing
-------

The tests still need fixing to work without vault,
I think the only way for that to happen would be to make the test install zabbix locally first, then run this against it?

Example Playbook
----------------

```
---
- hosts: zabbix
  roles:
    - role: zabbix-templates-role
```

License
-------

MIT

