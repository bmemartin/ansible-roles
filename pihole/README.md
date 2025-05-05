# Pi-hole

[Pi-hole](https://pi-hole.net) is a DNS sinkhole that protects your devices from unwanted content without installing any client-side software.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: pihole
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| pihole   | All tasks |
| update   | Update all components |

## ⌨️ Command-line Interface

Review the Pi-hole CLI documentation

```shell
pihole --help
```

```shell
pihole-FTL --help
```