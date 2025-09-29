# Docker

[Docker](https://www.docker.com) helps developers build, share, run, and verify applications anywhere — without tedious environment configuration or management.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: docker
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| docker | All tasks |
| update | Update all components |
