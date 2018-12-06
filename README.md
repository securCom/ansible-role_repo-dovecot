# Repo: Dovecot

Manage Dovecot community repositories to the supported systems.

# Requirements

Forr supported systems  see https://repo.dovecot.org/. If yhour system is not supported,
the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `dovecot_repo_version`: the dovecot version to install
- `dovecot_repo_state`: define presence of the repository

# Dependencies

There no external dependencies.

# Example Playbook

```
- hosts: servers
  roles:
     - securcom.repo_dovecot
```

# License

BSD

# Author Information


- Peter Hudec (@hudecof)