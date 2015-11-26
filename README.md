# README.md
# Ansible Role: mats116.td-agent2

An Ansible role that installs td-agent2 on **Ubuntu 14.04 LTS**

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

```yaml
td_agent_version: "2.2.1"
td_agent_user: root
td_agent_group: root
td_agent_plugins: []
```

## Dependencies

none

## Example Playbook

```yaml
- hosts: web-server
  roles:
    - role: mats116.td-agent2
      td_agent_plugins:
        - fluent-plugin-forest
```

## License

MIT
