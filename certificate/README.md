# Certificate

Certificate is a collection of tasks that generates OpenSSL certificates on the host.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  vars:
    certificate_path: /certs
  roles:
    - role: certificate
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| certificate | All tasks |
