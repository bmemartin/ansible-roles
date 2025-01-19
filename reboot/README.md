# Reboot

Reboot handles the rebooting of the host, if required.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: reboot
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| reboot | All tasks |
| update | All tasks |
