# AVD Testing

This repository contains a base data model for an L2LS design with 2 spines and 2 leaf pairs configured with MLAG. Adapt the data model as needed to test AVD features and the rendered EOS configs.

## Initial Topology

The initial startup topology is configured as an L2LS design, but can be modified as needed.

- (2) Spines
- (4) Leafs
- (2) SVIs - VLAN 10 and 20
- (2) Hosts

![L2LS Topology](/images/avd-testing-topo.png)

## Getting started

1. Make a copy of this repo template, by choosing `Use this template` and select `Create a new repository`
2. From the new repository, under `Code` choose `Create a Codespace` to launch a devcontainer.

This will launch a devcontainer in GitHub with VS Code and all the tools needed to run [AVD](https://avd.arista.com/). 

## Build Configs and Docs

From the terminal, you can run the build.yml playbook as shown below.

``` bash
# Option #1 - shortcut to run build playbook (see Makefile)
make build

# Option #2 - run ansible command directly
ansible-playbook playbooks/build.yml
```