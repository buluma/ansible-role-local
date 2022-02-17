# [local](#local)

Roles under testing [DO NOT USE]

|GitHub|GitLab|Quality|Downloads|Version|
|------|------|-------|---------|-------|
|[![github](https://github.com/buluma/ansible-role-local/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-local/actions)|[![gitlab](https://gitlab.com/buluma/ansible-role-local/badges/main/pipeline.svg)](https://gitlab.com/buluma/ansible-role-local)|[![quality](https://img.shields.io/ansible/quality/)](https://galaxy.ansible.com/buluma/local)|[![downloads](https://img.shields.io/ansible/role/d/)](https://galaxy.ansible.com/buluma/local)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-local.svg)](https://github.com/buluma/ansible-role-local/releases/)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.facts
      facts:
        - key: datacenter
          value: Amsterdam
        - key: availability_zone
          value: west
```


## [Role Variables](#role-variables)

The default values for the variables are set in `defaults/main.yml`:
```yaml
---
# defaults file for ansible-role-local
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-local/blob/main/requirements.txt).


## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.co.ke/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-local/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|alpine|all|
|amazon|Candidate|
|el|8|
|debian|all|
|fedora|all|
|opensuse|all|
|ubuntu|all|

The minimum version of Ansible required is 2.10, tests have been done to:

- The previous version.
- The current version.
- The development version.



If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-local/issues)

## [License](#license)

Apache-2.0

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
