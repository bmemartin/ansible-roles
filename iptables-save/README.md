# iptables-save

[iptables](https://www.netfilter.org/projects/iptables/index.html)-save is an Ansible handler used to persist iptables rule changes.

## 🚀 Usage

Define the [role dependency](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_reuse_roles.html#using-role-dependencies) in the `meta/main.yaml` file within the role directory.

```yaml
---
dependencies:
  - role: iptables-save
```

Tasks can trigger the handler by using `notify: save iptables`. For example:

```yaml
---
- name: Allow established and related incoming connections
  ansible.builtin.iptables:
    chain: INPUT
    ctstate:
      - ESTABLISHED
      - RELATED
    jump: ACCEPT
  notify: save iptables
```