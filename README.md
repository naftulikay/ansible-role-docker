# ansible-role-docker [![Build Status][svg:travis]][travis]

An Ansible role for installing, configuring, and starting Docker on a system.

Available on Ansible Galaxy at [`naftulikay.docker`][galaxy].

## Requirements

Officially tested operating systems are listed in the Galaxy manifest.

## Role Variables

None.

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

## License

MIT


 [svg:travis]: https://travis-ci.org/naftulikay/ansible-role-docker.svg?branch=master
 [travis]: https://travis-ci.org/naftulikay/ansible-role-docker
 [galaxy]: https://galaxy.ansible.com/naftulikay/docker/
