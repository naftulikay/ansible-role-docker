# ansible-role-docker [![Build Status][svg:travis]][travis]

An Ansible role for installing, configuring, and starting Docker on a system.

Available on Ansible Galaxy at [`naftulikay.docker`][galaxy].

## Requirements

Officially tested operating systems are listed in the Galaxy manifest.

## Role Variables

<dl>
  <dt><code>docker_users</code></dt>
  <dd>A string or list of strings of usernames to add to the <code>docker</code> group.</dd>
<dl>

## Dependencies

None.

## Example Playbook

Here are some example playbooks to get started with.

### Defaults

Simply get that Docker dockering:

```yaml
---
- name: install
  hosts: all
  become: true
  roles:
    - role: docker
```

Add the `vagrant` user to the `docker` group:

```yaml
---
- name: install
  hosts: all
  become: true
  roles:
    - role: docker
      docker_users: vagrant
```

## License

MIT


 [svg:travis]: https://travis-ci.org/naftulikay/ansible-role-docker.svg?branch=master
 [travis]: https://travis-ci.org/naftulikay/ansible-role-docker
 [galaxy]: https://galaxy.ansible.com/naftulikay/docker/
