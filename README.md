Installs the CISOfy Software - Lynis Community for RHEL.

Requirements
------------

This role only is needed/runs on RHEL and its derivatives.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):
```yaml
lynis_repofile_path: "/etc/yum.repos.d/cisofy-lynis.repo"

lynis_repo_url: "https://packages.cisofy.com/community/lynis/rpm/"
lynis_repo_gpgkey_url: "https://packages.cisofy.com/keys/cisofy-software-rpms-public.key"
lynis_repo_priority: 2
```
If for some reason you don't want to install lynis during the repo setup set following variable to `false`.

```yaml
lynis_install: false
```

Dependencies
------------

None.

Example Playbook
----------------
```yaml
- hosts: servers
  roles:
    - goathy.repo-lynis
```

License
-------

[MIT](./LICENSE)
