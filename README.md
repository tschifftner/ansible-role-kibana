# Ansible Role: Install Kibana 4.3.1+

[![Build Status](https://travis-ci.org/tschifftner/ansible-role-kibana.svg)](https://travis-ci.org/tschifftner/ansible-role-kibana)

Installs Kibana 4.3.1 from source on Debian/Ubuntu linux servers.

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
workspace: "/opt/kibana"
kibana_user: "kibana"
kibana_group: "kibana"
kibana_pid_file: "/var/run/kibana.pid"
kibana_server_port: "5601"
kibana_server_host: "0.0.0.0"
kibana_chmod: "0760"
kibana_current_dir: "current"
kibana_executable: "bin/kibana"
```

## Dependencies

None.

## Installation

```
$ ansible-galaxy install tschifftner.kibana
```

## Example Playbook

    - hosts: server
      roles:
        - { role: tschifftner.kibana }

## Supported OS
Ansible          | Debian Jessie    | Ubuntu 14.04
:--------------: | :--------------: | :-------------:
2.1              | Yes              | Yes

## License

MIT / BSD

## Author Information

 - [Tobias Schifftner](https://twitter.com/tschifftner), [ambimax® GmbH](https://www.ambimax.de)