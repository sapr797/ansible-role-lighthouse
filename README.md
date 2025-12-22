# Ansible Role: Lighthouse

Deploys Lighthouse web interface for ClickHouse using Docker.

## Requirements

- Ubuntu 20.04/22.04
- Ansible 2.9+
- Docker

## Role Variables

See `defaults/main.yml` for all available variables.

## Example Playbook

```yaml
- hosts: web_servers
  roles:
    - role: lighthouse
      vars:
        clickhouse_host: "clickhouse-server.example.com"
