# Ansible-role-sysctl

Role for manage sysctl rules

## Requirements

Tested with Ansible 1.9.5

## Role Variables
Available variables are listed below, along with default values (see `defaults/main.yml`):

    sysctl_rules:
      net.ipv4.ip_local_port_range: "1024 65000"
      vm.swappiness: "0"

Error on setting non-existent sysctl keys might be ignored with:

     sysctl_ignore_errors: "yes"

## Dependencies

None.

## Example Playbook

    - hosts: webserver
      roles:
        - sysctl

## License

MIT / BSD

## Author Information

This role was created in 2016 by [Meteor Liu](http://liusanjin.me/)
