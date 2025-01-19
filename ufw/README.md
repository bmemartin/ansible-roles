# UFW

[Uncomplicated Firewall (UFW)](https://manpages.ubuntu.com/manpages/bionic/en/man8/ufw.8.html) is a program for managing a Linux firewall and aims to provide an easy to use interface for the user.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: ufw
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| firewall | All tasks |
| update | Update all components |

## ⌨️ Command-line Interface

Review the UFW CLI documentation

```shell
ufw --help
```
