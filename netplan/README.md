# Netplan

[Netplan](https://netplan.io) is a utility for easily configuring networking on a linux system.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: netplan
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| netplan | All tasks |
