Podman
=========
[![Build Status](https://travis-ci.org/islander/ansible-role-podman.svg?branch=master)](https://travis-ci.org/islander/ansible-role-podman)

A role to install [podman][1] container engine.


Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```
podman_repo_url: "deb https://download.opensuse.org/repositories/devel:/kubic:/libcontainers:/stable/xUbuntu_{{ ansible_distribution_version }}/ /"
podman_sources_list: "/etc/apt/sources.list.d/devel:kubic:libcontainers:stable.list"
podman_key_url: "https://download.opensuse.org/repositories/devel:/kubic:/libcontainers:/stable/xUbuntu_{{ ansible_distribution_version }}/Release.key"
```

Example Playbook
----------------
Install role from galaxy: `ansible-galaxy install islander.podman`

    - hosts: servers
      roles:
         - islander.podman

License
-------

BSD

Author Information
------------------

This role was created by [kiba][2]

[1]: https://podman.io
[2]: https://kiba.io
