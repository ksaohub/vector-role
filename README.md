Role Name
=========

vector-role


Role Variables
--------------

You can specify a particular version (or `*` for the latest). Please note that downgrade isn't supported.
```yaml
vector_version: "0.24.0"
```

Example Playbook
----------------

```yaml
- name: Install Vector
  hosts: vector
  roles:
    - vector-role
```