Run Logikal Playbook
====================
GitHub Action for running a [Logikal Ansible
playbook](https://github.com/logikal-io/ansible-public-playbooks).

Usage
-----
```yaml
steps:
  - uses: logikal-io/run-logikal-playbook@v1
    with:
      roles: role1, role2, ...
      vars: '{"key1": "value1", "key2": "value2", ...}'
```

Inputs
------
`roles`: Required, a comma-separated list of the roles to run.
`vars`: Optional, the variables to set as a string-encoded JSON.

License
-------
This GitHub Action is licensed under the MIT open source license.
