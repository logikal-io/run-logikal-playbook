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
The available roles can be found in the
[ansible-public-playbooks](https://github.com/logikal-io/ansible-public-playbooks/tree/main/roles)
repository.

`vars`: Optional, the variables to set as a string-encoded JSON.
The available variables can be found in the `vars/main.yml` file of the appropriate role.

`version`: Optional, the
[ansible-public-playbooks](https://github.com/logikal-io/ansible-public-playbooks/releases)
repository version to use.

License
-------
This GitHub Action is licensed under the MIT open source license.
