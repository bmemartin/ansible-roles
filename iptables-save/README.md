# iptables-save

`iptables-save` provides Ansible handlers that persist current IPv4 and IPv6 firewall rules to disk using [iptables-save](https://www.netfilter.org/projects/iptables/index.html) and [ip6tables-save](https://www.netfilter.org/projects/iptables/index.html).

These handlers are typically triggered by other roles or tasks that modify iptables rules, ensuring changes are saved across system reboots.

## 🚀 Usage

Include this role as a [role dependency](https://docs.ansible.com/projects/ansible/latest/playbook_guide/playbooks_reuse_roles.html#using-role-dependencies) in your role's `meta/main.yml` file:

```yaml
---
dependencies:
  - role: iptables-save
```

Then, notify the handler(s) from any task that modifies iptables rules:

```yaml
---
- name: Allow established and related incoming connections
  ansible.builtin.iptables:
    chain: INPUT
    ctstate:
      - ESTABLISHED
      - RELATED
    jump: ACCEPT
  notify:
    - save iptables rules
    - save ip6tables rules
```
