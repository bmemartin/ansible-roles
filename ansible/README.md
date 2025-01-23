# Ansible

[Ansible](https://docs.ansible.com/ansible/latest/index.html) offers open-source automation that is simple, flexible, and powerful.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: ansible
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| ansible | All tasks |
| update | Update all components |
