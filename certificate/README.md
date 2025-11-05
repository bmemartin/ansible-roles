# Certificate

Certificate is a collection of tasks that generates OpenSSL certificates on the host.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: certificate
      vars:
        certificate_path: /certs
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| certificate | All tasks |
