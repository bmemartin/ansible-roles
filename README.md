# Ansible Roles

A collection of Ansible roles for automating host configuration and application deployment.

## 📦 Roles

- [Certificate](certificate/README.md)
- [Docker](docker/README.md)
- [Docker Compose](docker_compose/README.md)
- [Hostname](hostname/README.md)
- [iptables](iptables/README.md)
- [iptables-save](iptables-save/README.md)
- [Keepalived](keepalived/README.md)
- [kubectl](kubectl/README.md)
- [Netplan](netplan/README.md)
- [Packages](packages/README.md)
- [Pi-hole](pihole/README.md)
- [pipx](pipx/README.md)
- [PostgreSQL](postgresql/README.md)
- [Reboot](reboot/README.md)
- [SSH](ssh/README.md)
- [Time](time/README.md)
- [Unbound](unbound/README.md)

## 🖥️ Platforms

### [Ubuntu](https://ubuntu.com)

- 24.04 (Noble Numbat)

## 🔧 Setup

### Ansible collections

Install the required Ansible collections:

```shell
ansible-galaxy collection install -r requirements.yaml
```

## ✅ Testing

Create the Ansible `hosts` file with the desired host entries.

Execute all playbooks with the following command:

```shell
ANSIBLE_HOST_KEY_CHECKING=false \
ANSIBLE_ROLES_PATH=. \
ansible-playbook --inventory hosts playbooks/playbook.yaml
```
