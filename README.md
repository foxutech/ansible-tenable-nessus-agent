Nessus Agent Ansible Role
=========================

## Purpose

Helps automating the deployment and configuration of the [Nessus Agent](https://www.tenable.com/products/nessus/nessus-agents).

## Supported Platforms

See [meta info](meta/main.yml).

## User Manual

### How to use

* Add the role to your project's Ansible galaxy requirements file and install it via the ansible-galaxy command
```
- src: git+https://github.com/polster/ansible-nessus-agent.git
  name: "nessus-agent"
  version: "v1.0.0"
```
* Add the following line to your Ansible playbook's role section as follows (sample):
```
roles:
    - role: nessus-agent
```

## Configuration

### <a name="configVariables"></a>Configurable variables

See [defaults](defaults/main.yml)
