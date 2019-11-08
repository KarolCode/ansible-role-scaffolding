# Ansible Role Scaffolding

Short description of the role.

## Supported distributions:

  * Debian
  * Ubuntu
  * CentOS
  * Fedora

## Install role:

### From Ansible Galaxy:

1. Put in to file `requirements.yml`:

```yaml
- name: <ROLE_NAME>
  src: <OWER>.<ROLE NAME>
  version: v<VERSION>
```

2. Run command: `ansible-galaxy install -r requirements.yml`
### From GitHub:

1. Put in to file `requirements.yml`:

```yaml
- name: <ROLE_NAME>
  src: git@bitbucket.org:<OWER>/<ROLE_NAME>.git
  scm: git
  version: v<VERSION>
```

```yaml
- name: <ROLE_NAME>
  src: https://github.com/<OWER>/<ROLE_NAME>
  scm: git
  version: v<VERSION>
```

2. Run command: `ansible-galaxy install -r requirements.yml`

## Application example:

```yaml
  tasks:

    - name: Role....
      import_role:
        name: <ROLE_NAME>
      tags:
        - <ROLE NAME>
```
