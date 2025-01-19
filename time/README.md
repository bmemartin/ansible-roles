# Time

Time is a collection of tasks that configures the hosts timezone and network time protocol server(s).

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: time
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| time | All tasks |
