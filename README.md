Nessus Agent Ansible Role
=========================

## Purpose

Helps automating the deployment and configuration of the [Nessus Agent](https://www.tenable.com/products/nessus/nessus-agents).

## Supported Platforms

See [meta info](meta/main.yml).

## User Manual

### Basic usage

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

### Deploy and pair

* Pass in the following values in order to deploy and link the agent (sample values):
```
roles:
    - role: nessus-agent
      nessus_agent_key: "sdfasdjfee4545345345gasdgsag"
      nessus_agent_name: "osx-server01.tinkerstest.com"
      nessus_agent_host_name: "nessus-manager.tinkerstest.com"
      nessus_agent_host_port: "443"
      nessus_agent_link: true
```

## Configuration

### <a name="configVariables"></a>Configurable variables

See [defaults](defaults/main.yml)
