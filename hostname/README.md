# Hostname

Hostname is a collection of tasks that configures the hosts hostname.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: hostname
```

### Configuration

The Ansible inventory is used as the source of all configuration.

### Tags

| Tag | Description |
| --- | ----------- |
| hostname | All tasks |
