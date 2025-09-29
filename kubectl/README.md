# kubectl

[kubectl](https://kubernetes.io/docs/reference/kubectl) is a command line tool for communicating with a Kubernetes cluster's control plane, using the Kubernetes API.

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: kubectl
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| kubectl | All tasks |
| update | Update all components |
