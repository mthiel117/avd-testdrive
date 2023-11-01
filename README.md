# AVD Testing

This repository contains a base data model for an L2LS design with 2 spines and 2 leaf pairs configured with MLAG. Adapt the data model as needed to test AVD features and the rendered EOS configs.

## Initial Topology

The initial startup topology is configured as an L2LS design, but can be modified as needed.

- (2) Spines
- (4) Leafs
- (2) SVIs - VLAN 10 and 20
- (2) Hosts

![L2LS Topology](/images/avd-testing-topo.png)

## Build Configs and Docs

``` bash
make build
```