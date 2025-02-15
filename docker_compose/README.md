# Docker Compose

Docker Compose is a collection of tasks that establishes, and starts, a [Compose](https://docs.docker.com/compose) project on the target host(s).

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  gather_facts: true
  roles:
    - role: docker_compose
      vars:
        docker_compose_path: /project
```

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| docker_compose | All tasks |
| docker_compose_up | Recreate containers even if their configuration and image haven't changed. It must be explicitly specified to activate. |
