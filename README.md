[![Build Status](https://www.travis-ci.org/securCom/ansible-role_repo-dovecot.svg?branch=master)](https://www.travis-ci.org/securCom/ansible-role_repo-dovecot)


# Repo: Dovecot

Manage Dovecot community repositories.

# Requirements

For supported systems  see https://repo.dovecot.org/. If yhour system is not supported,
the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `dovecot_repo_version`: the dovecot version to install
- `dovecot_repo_state`: define presence of the repository

# Dependencies

There no external dependencies.

# Example Playbook

To install role, add following line to **ansible-galaxy** requirements file
```
- src: https://github.com/securCom/ansible-role_repo-dovecot
  version: master
  name: securcom.repo_dovecot
```

```
- hosts: servers
  roles:
     - securcom.repo_dovecot
```

# License

BSD

# Author Information


- Peter Hudec (@hudecof)