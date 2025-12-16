# pipx

[pipx](https://pipx.pypa.io) is a tool to help you install and run end-user applications written in Python.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: pipx
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| pipx | All tasks |
| update | Update all components |
