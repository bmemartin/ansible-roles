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

## 🪵 Logs and Status

The Unbound configuration allows for the definition of a logfile to which logs are written. If unspecified, logs will be written to syslog and can be found as per below.

Show logs from the unbound service

```shell
journalctl -u unbound
```

Show runtime status of the unbound service

```shell
systemctl status unbound
```
