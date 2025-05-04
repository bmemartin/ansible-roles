# iptables

[iptables](https://www.netfilter.org/projects/iptables/index.html) is the userspace command line program used to configure the Linux 2.4.x and later packet filtering ruleset.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: iptables
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| firewall | All tasks |
| iptables | All tasks |
| update | Update all components |

## ⌨️ Command-line Interface

Review the iptables CLI documentation

```shell
iptables --help
```
