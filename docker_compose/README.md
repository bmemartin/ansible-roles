# Docker Compose

Docker Compose is a collection of tasks that defines and runs a [Compose](https://docs.docker.com/compose) project on the target host(s).

## 🚀 Usage

Minimal Ansible playbook

```yaml
---
- hosts: all
  gather_facts: true
  vars:
    docker_compose_path: /project
  roles:
    - role: docker_compose
```

> [!TIP]
> Use `--extra-vars docker_compose_pull=always` at runtime to ensure images are refreshed during upgrades, especially when relying on tags like `latest`.
>
> Use `--extra-vars docker_compose_recreate=always` at runtime to ensure project containers are always recreated.

### Configuration

Available configuration options, along with default values, are documented in [defaults/main.yaml](defaults/main.yaml).

### Tags

| Tag | Description |
| --- | ----------- |
| docker_compose | All tasks |
