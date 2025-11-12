# Keepalived

[Keepalived](https://www.keepalived.org/index.html) is used to provide simple and robust facilities for loadbalancing and high-availability to Linux system and Linux based infrastructures.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  vars:
    keepalived_vrrp_instances:
      - name: demo
        state: MASTER
        interface: '{{ ansible_default_ipv4.interface }}'
        priority: 255
        virtual_ipaddress: 192.168.0.244/24
  roles:
    - role: keepalived
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| keepalived | All tasks |
