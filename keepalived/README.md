# Keepalived

[Keepalived](https://www.keepalived.org/index.html) is used to provide simple and robust facilities for loadbalancing and high-availability to Linux system and Linux based infrastructures.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: keepalived
      vars:
        keepalived_vrrp_instances:
          - name: demo
            virtual_ipaddress: 192.168.10.10
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| keepalived | All tasks |
| firewall | Applies the firewall rule tasks |
| iptables | Applies the iptables rule tasks |
