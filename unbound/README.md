# Unbound

[Unbound](https://unbound.docs.nlnetlabs.nl/en/latest) is a validating, recursive, caching DNS resolver.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: unbound
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| unbound | All tasks |
| update | Update all components |
